# Java Banking Engine

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-%23ED8B00?style=for-the-badge&logo=java" alt="Java 17" />
  <img src="https://img.shields.io/badge/Spring%20Boot-3.x-%236DB33F?style=for-the-badge&logo=spring" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/OpenAPI-3.x-%236BA0D8?style=for-the-badge&logo=openapiinitiative" alt="OpenAPI" />
  <img src="https://img.shields.io/badge/Microservices-Architecture-8A2BE2?style=for-the-badge&logo=apache" alt="Microservices" />
</p>

## Descripción

Este repositorio documenta un recorrido de aprendizaje para construir una plataforma bancaria moderna con Java y Spring. El enfoque principal es desarrollar un sistema financiero paso a paso, aplicando buenas pr?cticas de arquitectura, backend y despliegue.

## Objetivo

Crear una experiencia completa de desarrollo backend orientada a banca digital, cubriendo desde dise?o de APIs hasta microservicios distribuidos y entrega en entornos de producci?n.

## Roadmap del proyecto

### Proyecto 1 - API First y contratos OpenAPI

Diseñar contratos YAML, endpoints REST, esquemas de request/response, headers, errores y versionamiento, usando Party Reference Data Directory de BIAN 14.0.0.

> Java no es necesario hoy. El alumno aprende a dise?ar antes de programar.

### Proyectos 2 a 8 - Un microservicio por proyecto

Cada proyecto incorpora un microservicio que permanece en el producto final. Los temas del módulo se practican sobre una capacidad concreta de la plataforma bancaria.

| Proyecto | Microservicio | Responsabilidad en el producto | Temas principales | SD BIAN 14.0.0 de referencia |
| --- | --- | --- | --- | --- |
| 2. Java y Spring Boot | Customer Service | Registrar, consultar y actualizar clientes; gestionar su estado. | Java, POO, Collections, excepciones, Git, Maven, Spring Boot, validaciones, JPA, PostgreSQL y Flyway. | Party Reference Data Directory: identificación y datos de contacto. |
| 3. Arquitectura y testing | Account Service | Abrir cuentas corrientes, gestionar estados y proteger las reglas de saldo y movimientos. | Arquitectura hexagonal, SOLID, Value Objects, patrones, JUnit, Mockito y Testcontainers. | Current Account: ciclo de vida y operaciones de cuentas corrientes. |
| 4. Integraciones bancarias | Banking Experience Service | Ofrecer una API para canales digitales que integre clientes, cuentas y un legado simulado. | Clientes OpenAPI, Feign/WebClient, REST/SOAP, Oracle, PL/SQL, OAuth2/JWT, trazabilidad y pruebas contractuales. | Composición de Party Reference Data Directory y Current Account; sin un SD propio equivalente. |
| 5. Reactividad y Quarkus | Notification Service | Procesar eventos y enviar notificaciones de aperturas de cuentas y resultados de transferencias. | Quarkus, Mutiny, Uni/Multi, composición asíncrona, errores y backpressure; laboratorio comparativo Reactor/WebFlux. | Correspondence: alineación parcial para comunicaciones salientes. |
| 6. Sistemas distribuidos | Transfer Service | Coordinar transferencias entre cuentas, evitar duplicados y recuperar operaciones ante fallos. | Eventos, Saga, Outbox, idempotencia, concurrencia, resiliencia y observabilidad. | Payment Order Initiation: captura e iniciación de la orden; Saga y ejecución interna son decisiones de implementación. |
| 7. Azure y DevSecOps | Audit Service | Recibir, conservar y consultar eventos de auditoría de clientes y operaciones. | Docker, Kubernetes, AKS, CI/CD, SonarQube, análisis de seguridad, Key Vault y monitoreo. | Customer Event History: alineación parcial con el historial de eventos del cliente. |
| 8. Reto integrador | Statement Service | Solicitar, generar y consultar estados de cuenta de forma asíncrona. | System Design, rendimiento, SQL, seguridad, pruebas de carga, code review y defensa arquitectónica. | Document Services: generación documental; Current Account como fuente de movimientos. |

### Alcance del mapeo BIAN

SD significa **Service Domain**. La columna propone una alineación funcional para el aprendizaje; no implica conformidad completa con BIAN ni una equivalencia obligatoria entre un SD y un microservicio. Banking Experience compone dominios. Audit cubre historial funcional del cliente; la auditoría técnica, los logs y las trazas son capacidades transversales.

Referencia obligatoria para todos los proyectos: **BIAN 14.0.0**. Consultar el [Service Landscape 14](https://bian.org/servicelandscape-14-0-0/) y las [APIs oficiales de la release 14.0.0](https://github.com/bian-official/public/tree/main/release14.0.0). Cada contrato debe declarar SD, Control Record, versión de referencia, fuente oficial y simplificaciones. La versión propia de la API y la versión OpenAPI se gestionan por separado.

### Evolución de la plataforma

- Cada proyecto entrega su servicio ejecutable, documentado e integrado con los anteriores.
- Cada servicio es dueño de sus datos y se integra mediante contratos API o eventos.
- Los contratos de servicios futuros pueden simularse para avanzar sin implementarlos antes de tiempo.
- Los servicios anteriores reciben ajustes necesarios para la integración. Account Service incorporará operaciones seguras de débito, crédito o reserva de fondos al integrar Transfer Service.
- Las prácticas de arquitectura, pruebas, seguridad y documentación se acumulan en los siguientes proyectos.
- Notification Service utiliza Quarkus y Mutiny; Reactor/WebFlux se aborda en un laboratorio comparativo acotado.
- El proyecto 7 despliega todo el ecosistema existente en Azure, además de construir Audit Service.
- El proyecto 8 incorpora Statement Service y valida el recorrido completo: registrar un cliente, abrir cuentas, transferir fondos, recibir notificaciones y generar un estado de cuenta con auditoría y trazabilidad.
- La autenticación se integra con un proveedor de identidad OAuth2/OIDC y el API Gateway se configura como infraestructura de acceso.

## Stack principal

- Java 17
- Spring Boot 3
- OpenAPI / Swagger
- Maven / Gradle
- JUnit / Mockito
- PostgreSQL / Oracle / PL/SQL
- Docker / Kubernetes
- Azure DevOps / GitHub Actions
- OAuth2 / JWT
- Microservicios y event-driven architecture
- Quarkus

## Recomendación

Este proyecto es ideal para personas que desean aprender backend enterprise con un enfoque pr?ctico y aplicado al mundo bancario.

## Licencia

Este repositorio est? pensado como material de aprendizaje y desarrollo personal.
