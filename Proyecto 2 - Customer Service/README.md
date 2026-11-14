# Proyecto 2 - Customer Service

Implementar un microservicio de clientes con Java 21, Spring Boot, Maven, PostgreSQL, JPA y Flyway a partir de [este contrato OpenAPI](contracts/customer-service-bian.yaml).

## Alcance

Registro, consulta, actualización de datos y activación/desactivación de personas naturales. Cuentas, saldos, transferencias, preferencias comerciales y KYC pertenecen a otros módulos.

| Método | Ruta relativa a /banking/v1 | Operación |
| --- | --- | --- |
| POST | /PartyReferenceDataDirectory/Register | Register |
| GET | /PartyReferenceDataDirectory/{partyreferencedatadirectoryid}/Retrieve | Retrieve |
| PUT | /PartyReferenceDataDirectory/{partyreferencedatadirectoryid}/Update | Update |
| PUT | /PartyReferenceDataDirectory/{partyreferencedatadirectoryid}/Control | Control |

## Alineación BIAN

Referencia fijada: [Party Reference Data Directory, BIAN 14.0.0](https://github.com/bian-official/public/blob/main/release14.0.0/semantic-apis/oas3%20/yamls/PartyReferenceDataDirectory.yaml). Se utilizan el SD, el CR y cuatro acciones oficiales como base. Esta es una adaptación educativa parcial: DTOs propios, personas naturales únicamente, sin Behavior Qualifiers y registro con HTTP 201 en lugar del 200 de referencia. No representa una API oficial certificada.

El proyecto 1 y este servicio utilizan Party Reference Data Directory de BIAN 14.0.0. Este contrato acota la implementación a identidad, contacto y estado del cliente; las extensiones didácticas del proyecto 1 no se incorporan automáticamente.

## Reglas para implementar

- Generar UUID y fechas UTC en el servidor. Registrar clientes en ACTIVE.
- Hacer única la combinación de tipo, número y país del documento mediante restricción de base de datos; convertir violaciones concurrentes a HTTP 409. No se reutiliza el documento de un cliente inactivo.
- Update reemplaza person y contact; identificación y estado no se actualizan por esta operación. Las escrituras concurrentes usan última escritura en esta etapa.
- Control cambia ACTIVE/INACTIVE, requiere motivo y conserva el registro. Repetir el estado actual no altera updatedAt. No cierra cuentas ni elimina obligaciones; la integración con cuentas se incorpora posteriormente.
- Rechazar fechas de nacimiento presentes o futuras y datos inválidos. No registrar documentos, correos ni tokens en logs.
- Propagar X-Correlation-ID y devolver errores application/problem+json con formato Problem Details.
- JWT y permisos customers:read/customers:write forman parte del contrato objetivo. En este módulo pueden usarse tokens de desarrollo firmados; la integración completa con proveedor OAuth2/OIDC se realiza en Proyecto 4.

## Criterios de aceptación

- Registrar devuelve 201, Location y el registro persistido; documento duplicado devuelve 409.
- Consultar un UUID existente devuelve 200; uno inexistente, 404; uno mal formado, 400.
- Actualizar sustituye datos personales/contacto sin cambiar identificación ni estado.
- Desactivar/reactivar conserva datos y respeta la semántica de repetición.
- Validaciones, autenticación y autorización producen los errores documentados.
- El recorrido registro → consulta → actualización → desactivación funciona contra PostgreSQL.

Este directorio contiene el contrato y el alcance; la aplicación Java todavía debe implementarse.
