# Java Backend Engineering Academy

> Programa de formación profesional: De Java Fundamentals a Senior Backend Engineering.
>
> Especialización en Java, Spring Boot, Quarkus, Microservicios, Arquitectura Bancaria, API First, Azure y DevSecOps.

## 1. Información general

| Campo                     | Descripción                                         |
| ------------------------- | --------------------------------------------------- |
| Programa                  | Java Backend Engineering Academy                    |
| Nivel                     | Fundamentals → Junior → Mid → Senior                |
| Duración estimada         | 32–40 semanas                                       |
| Dedicación                | 10–12 horas semanales                               |
| Modalidad                 | Teoría, laboratorios, proyectos y evaluaciones      |
| Lenguaje principal        | Java 21 LTS                                         |
| Versiones complementarias | Java 8, 11 y 17                                     |
| Frameworks                | Spring Boot, Spring Security, Spring Cloud, Quarkus |
| Arquitectura              | REST, Microservicios, Hexagonal, DDD                |
| Cloud                     | Microsoft Azure                                     |
| Especialización           | Backend empresarial y bancario                      |

### Objetivo general

Formar desarrolladores backend capaces de diseñar, implementar, integrar, probar y desplegar soluciones empresariales utilizando Java y tecnologías modernas.

El programa está orientado a competencias técnicas utilizadas en organizaciones financieras como BCP, BBVA, Interbank y consultoras tecnológicas.

Completar el programa no garantiza alcanzar un puesto Senior; ese nivel requiere también experiencia profesional, autonomía y criterio técnico.

---

# 2. Malla curricular

## Proyecto 01 — API First & Contract Design

**Duración:** 3 semanas  
**Nivel:** Fundamentals / Junior

### Objetivo

Aprender a diseñar contratos de APIs empresariales antes de implementar código.

### Temario

1. Introducción a las APIs.
2. Arquitectura cliente-servidor.
3. Protocolo HTTP y HTTPS.
4. Métodos GET, POST, PUT, PATCH y DELETE.
5. Códigos de respuesta HTTP.
6. REST y principios de diseño.
7. API First vs. Code First.
8. Introducción a OpenAPI 3.x.
9. Sintaxis YAML y JSON.
10. Diseño de endpoints REST.
11. Paths, parameters y headers.
12. Request Body y Response Body.
13. Schemas y componentes reutilizables.
14. Validación de contratos.
15. Catálogos de errores.
16. Seguridad declarativa: OAuth2, JWT y API Keys.
17. Versionamiento de APIs.
18. Paginación, filtros y ordenamiento.
19. Idempotencia.
20. Introducción a BIAN.
21. Convenciones de nomenclatura.
22. Documentación con Swagger.
23. Pruebas con Postman.
24. Revisión y gobierno de contratos.

### Proyecto práctico

**Banking Customer API**

Diseñar contratos para las siguientes operaciones:

- Consultar cliente.
- Registrar cliente.
- Consultar cuentas.
- Consultar movimientos.
- Actualizar información del cliente.

### Entregables

- `customer-api.yaml`
- `api-guidelines.md`
- `error-catalog.md`
- Colección Postman.
- README técnico.
- Defensa del contrato API.

### Documentación

- [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Learn OpenAPI](https://learn.openapis.org/)
- [Swagger Documentation](https://swagger.io/docs/)
- [HTTP Semantics - RFC 9110](https://www.rfc-editor.org/rfc/rfc9110)
- [BIAN](https://bian.org/)

---

## Proyecto 02 — Java Core & Spring Boot

**Duración:** 5 semanas  
**Nivel:** Junior

### Objetivo

Implementar el contrato anterior mediante Java y Spring Boot, dominando fundamentos del lenguaje y programación orientada a objetos.

### Temario

#### Java Fundamentals

1. JDK, JVM y JRE.
2. Instalación y configuración de Java.
3. IntelliJ IDEA.
4. Variables y tipos de datos.
5. Operadores y estructuras de control.
6. Métodos y sobrecarga.
7. Clases y objetos.
8. Encapsulamiento.
9. Abstracción.
10. Herencia.
11. Polimorfismo.
12. Interfaces.
13. Clases abstractas.
14. Excepciones personalizadas.
15. Collections Framework.
16. Generics.
17. Optional.
18. Lambdas.
19. Streams API.
20. Programación funcional.
21. Records y características modernas de Java.
22. Manejo de fechas.
23. BigDecimal para operaciones financieras.

#### Herramientas

24. Git y control de versiones.
25. Branching y Pull Requests.
26. Maven y ciclo de compilación.
27. Gestión de dependencias.

#### Spring Boot

28. Spring Framework.
29. Inversión de control.
30. Inyección de dependencias.
31. Spring Beans.
32. Spring Boot Starters.
33. Controllers y Services.
34. DTOs y mappers.
35. Validaciones.
36. Manejo global de excepciones.
37. Spring Data JPA.
38. Hibernate.
39. Relaciones entre entidades.
40. Configuración por perfiles.
41. Flyway y migraciones.

### Proyecto práctico

Implementar Banking Customer API utilizando Java, Spring Boot y PostgreSQL.

### Entregables

- Aplicación Spring Boot.
- Endpoints funcionales.
- Persistencia relacional.
- Validaciones.
- Manejo de errores.
- Documentación técnica.
- Repositorio Git.

### Documentación

- [Dev.java](https://dev.java/learn/)
- [Java API Documentation](https://docs.oracle.com/en/java/javase/21/docs/api/)
- [Spring Boot](https://docs.spring.io/spring-boot/reference/)
- [Spring Data JPA](https://docs.spring.io/spring-data/jpa/reference/)
- [Maven](https://maven.apache.org/guides/)
- [Git Documentation](https://git-scm.com/doc)

---

## Proyecto 03 — Clean Architecture & Testing

**Duración:** 4 semanas  
**Nivel:** Junior avanzado / Mid

### Objetivo

Transformar la API en una solución mantenible mediante arquitectura hexagonal, principios SOLID y pruebas automatizadas.

### Temario

1. Clean Code.
2. Principios SOLID.
3. Single Responsibility Principle.
4. Open/Closed Principle.
5. Liskov Substitution Principle.
6. Interface Segregation Principle.
7. Dependency Inversion Principle.
8. Arquitectura en capas.
9. Arquitectura hexagonal.
10. Domain Layer.
11. Application Layer.
12. Infrastructure Layer.
13. Puertos de entrada y salida.
14. Adaptadores REST.
15. Adaptadores de persistencia.
16. Patrón Repository.
17. Patrón Factory.
18. Patrón Strategy.
19. Patrón Adapter.
20. Patrón Builder.
21. Introducción a DDD.
22. Entidades y Value Objects.
23. JUnit 5.
24. Mockito.
25. Mock y Spy.
26. Pruebas unitarias.
27. Pruebas de integración.
28. Testcontainers.
29. Cobertura de pruebas.
30. Code Review.
31. Refactorización.
32. Architecture Decision Records (ADR).

### Proyecto práctico

Refactorizar Banking Customer API utilizando arquitectura hexagonal.

### Entregables

- Separación por capas.
- Interfaces y puertos.
- Adaptadores.
- Pruebas unitarias.
- Pruebas de integración.
- Documentación arquitectónica.
- ADRs.

### Documentación

- [JUnit 5](https://junit.org/junit5/docs/current/user-guide/)
- [Mockito](https://site.mockito.org/)
- [Testcontainers](https://java.testcontainers.org/)
- [Martin Fowler](https://martinfowler.com/)
- [C4 Model](https://c4model.com/)

---

## Proyecto 04 — Banking Microservices & Integrations

**Duración:** 5 semanas  
**Nivel:** Mid-Level

### Objetivo

Implementar microservicios empresariales con integración entre APIs, seguridad y bases de datos.

### Temario

1. Arquitectura de microservicios.
2. Monolito vs. microservicios.
3. Separación por responsabilidades.
4. Microservicios UX y BS como patrón de referencia.
5. API Gateway.
6. Contratos OpenAPI.
7. OpenAPI Generator.
8. Generación de clientes HTTP.
9. Spring Cloud OpenFeign.
10. WebClient.
11. Retrofit.
12. Consumo de APIs REST.
13. Integración SOAP.
14. XML y WSDL.
15. Spring Security.
16. OAuth2.
17. OpenID Connect.
18. JWT.
19. Scopes y roles.
20. Headers corporativos.
21. Correlation ID.
22. Manejo de timeouts.
23. Oracle Database.
24. PL/SQL.
25. Stored Procedures.
26. Packages.
27. Azure SQL.
28. Integración con sistemas legados.
29. BIAN Service Domains.
30. Pruebas contractuales.

### Proyecto práctico

Construir dos microservicios:

**Customer UX API**

- Expone servicios a consumidores.
- Valida solicitudes.
- Consume APIs de negocio.
- Adapta respuestas.

**Customer BS API**

- Ejecuta casos de uso.
- Aplica reglas de negocio.
- Consulta datos.
- Integra servicios externos.

### Entregables

- Dos microservicios.
- Contratos OpenAPI.
- Clientes HTTP.
- Seguridad.
- Persistencia.
- Pruebas de integración.

### Documentación

- [Spring Security](https://docs.spring.io/spring-security/reference/)
- [Spring Cloud](https://spring.io/projects/spring-cloud)
- [OpenAPI Generator](https://openapi-generator.tech/)
- [OAuth2 - RFC 6749](https://www.rfc-editor.org/rfc/rfc6749)
- [Oracle Database](https://docs.oracle.com/en/database/)
- [BIAN](https://bian.org/)

---

## Proyecto 05 — Reactive Programming & Quarkus

**Duración:** 4 semanas  
**Nivel:** Mid-Level avanzado

### Objetivo

Comprender la programación reactiva y desarrollar servicios Java utilizando WebFlux y Quarkus.

### Temario

1. Programación imperativa.
2. Programación declarativa.
3. Programación funcional.
4. Programación reactiva.
5. Reactive Streams.
6. Publisher y Subscriber.
7. Mono.
8. Flux.
9. Operadores map y flatMap.
10. filter, zip y merge.
11. Manejo de errores reactivos.
12. Backpressure.
13. Spring WebFlux.
14. WebClient reactivo.
15. StepVerifier.
16. RxJava.
17. Single, Maybe y Observable.
18. Flowable.
19. Introducción a Quarkus.
20. CDI e inyección de dependencias.
21. Quarkus REST.
22. REST Client.
23. Mutiny.
24. Uni y Multi.
25. Comparación Spring Boot vs. Quarkus.
26. Rendimiento y consumo de recursos.

### Proyecto práctico

Crear una API reactiva de consultas bancarias y una implementación equivalente con Quarkus.

### Entregables

- Servicio WebFlux.
- Servicio Quarkus.
- Pruebas reactivas.
- Comparación técnica.
- Documentación de decisiones.

### Documentación

- [Project Reactor](https://projectreactor.io/docs/core/release/reference/)
- [Spring WebFlux](https://docs.spring.io/spring-framework/reference/web/webflux.html)
- [Quarkus Guides](https://quarkus.io/guides/)
- [SmallRye Mutiny](https://smallrye.io/smallrye-mutiny/)

---

## Proyecto 06 — Distributed Systems & Resilience

**Duración:** 5 semanas  
**Nivel:** Senior técnico

### Objetivo

Diseñar sistemas distribuidos resistentes a fallos y capaces de procesar operaciones financieras.

### Temario

1. Fundamentos de sistemas distribuidos.
2. Comunicación síncrona y asíncrona.
3. Event-Driven Architecture.
4. Apache Kafka.
5. Producers y Consumers.
6. Azure Service Bus.
7. Consistencia eventual.
8. Transacciones distribuidas.
9. Patrón Saga.
10. Orquestación.
11. Coreografía.
12. Temporal Workflows.
13. Compensaciones.
14. Idempotencia.
15. Patrón Outbox.
16. Retry.
17. Timeout.
18. Circuit Breaker.
19. Resilience4j.
20. Redis.
21. Caché e invalidación.
22. Concurrencia.
23. Optimistic Locking.
24. Pessimistic Locking.
25. Distributed Tracing.
26. OpenTelemetry.
27. Logs estructurados.
28. Métricas.
29. Manejo de fallos.
30. Pruebas de resiliencia.

### Proyecto práctico

Implementar un motor de transferencias bancarias con manejo de operaciones duplicadas, compensaciones y recuperación ante fallos.

### Entregables

- Microservicios distribuidos.
- Mensajería.
- Idempotencia.
- Saga.
- Trazabilidad.
- Pruebas de fallos.

### Documentación

- [Apache Kafka](https://kafka.apache.org/documentation/)
- [Temporal](https://docs.temporal.io/)
- [Resilience4j](https://resilience4j.readme.io/)
- [OpenTelemetry](https://opentelemetry.io/docs/)
- [Azure Service Bus](https://learn.microsoft.com/en-us/azure/service-bus-messaging/)

---

## Proyecto 07 — Azure Cloud & DevSecOps

**Duración:** 5 semanas  
**Nivel:** Mid / Senior

### Objetivo

Automatizar la construcción, validación y publicación de aplicaciones Java en Azure.

### Temario

1. Fundamentos de Cloud Computing.
2. Azure Resource Groups.
3. Azure Container Registry.
4. Docker.
5. Dockerfile.
6. Docker Compose.
7. Kubernetes.
8. Pods.
9. Deployments.
10. Services.
11. ConfigMaps.
12. Secrets.
13. Azure Kubernetes Service.
14. Azure API Management.
15. Azure Key Vault.
16. Azure DevOps Repos.
17. Azure Pipelines.
18. Jenkins.
19. GitHub Actions.
20. Integración continua.
21. Despliegue continuo.
22. SonarQube.
23. Quality Gates.
24. Análisis SAST.
25. Fortify.
26. Artifactory.
27. Análisis de dependencias.
28. Observabilidad.
29. Azure Monitor.
30. Application Insights.
31. Blue-Green Deployment.
32. Canary Deployment.
33. Rollback.
34. Gestión de configuración.
35. Seguridad de secretos.

### Proyecto práctico

Desplegar el ecosistema bancario en Azure con CI/CD y controles de calidad.

### Entregables

- Imágenes Docker.
- Manifiestos Kubernetes.
- Pipeline YAML.
- Quality Gates.
- Configuración segura.
- Monitoreo.
- Manual de despliegue.

### Documentación

- [Microsoft Azure](https://learn.microsoft.com/en-us/azure/)
- [Azure Kubernetes Service](https://learn.microsoft.com/en-us/azure/aks/)
- [Azure DevOps](https://learn.microsoft.com/en-us/azure/devops/)
- [Docker](https://docs.docker.com/)
- [Kubernetes](https://kubernetes.io/docs/)
- [SonarQube](https://docs.sonarsource.com/)
- [Azure Key Vault](https://learn.microsoft.com/en-us/azure/key-vault/)

---

## Proyecto 08 — Senior Backend Engineering Challenge

**Duración:** 5 semanas  
**Nivel:** Senior / Software Architecture

### Objetivo

Demostrar criterio técnico para diseñar, justificar y evolucionar sistemas backend empresariales.

### Temario

1. System Design.
2. Requerimientos funcionales.
3. Requerimientos no funcionales.
4. Escalabilidad.
5. Alta disponibilidad.
6. Tolerancia a fallos.
7. CAP Theorem.
8. Consistencia distribuida.
9. Domain-Driven Design.
10. Bounded Contexts.
11. Arquitectura empresarial.
12. C4 Model.
13. Diagramas de contexto.
14. Diagramas de contenedores.
15. Diagramas de componentes.
16. Architecture Decision Records.
17. Trade-offs arquitectónicos.
18. JVM Performance.
19. Garbage Collection.
20. Profiling.
21. Optimización SQL.
22. Índices y planes de ejecución.
23. Seguridad OWASP.
24. OAuth2 avanzado.
25. Code Review.
26. Gestión de deuda técnica.
27. Liderazgo técnico.
28. Mentoring.
29. Análisis de incidentes.
30. Postmortems.
31. Live Coding.
32. Entrevistas técnicas Senior.
33. Defensa de arquitectura.

### Proyecto práctico

Diseñar y defender una plataforma bancaria que integre clientes, cuentas, transferencias, seguridad, auditoría y monitoreo.

### Entregables

- Arquitectura completa.
- Código funcional.
- Diagramas C4.
- ADRs.
- Pruebas.
- Pipeline.
- Documentación.
- Defensa técnica.

### Documentación

- [C4 Model](https://c4model.com/)
- [OWASP API Security](https://owasp.org/www-project-api-security/)
- [Microsoft Azure Architecture Center](https://learn.microsoft.com/en-us/azure/architecture/)
- [Java Performance](https://docs.oracle.com/en/java/javase/21/gctuning/)
- [Martin Fowler](https://martinfowler.com/)

---

# 3. Documentación obligatoria por proyecto

Cada proyecto debe incluir:

| Archivo         | Descripción                     |
| --------------- | ------------------------------- |
| README.md       | Presentación y ejecución        |
| requirements.md | Requerimientos                  |
| openapi.yaml    | Contratos API                   |
| architecture.md | Diseño de arquitectura          |
| adr/            | Decisiones arquitectónicas      |
| testing.md      | Estrategia de pruebas           |
| security.md     | Seguridad                       |
| deployment.md   | Despliegue                      |
| interview.md    | Preguntas y respuestas técnicas |

## Estructura recomendada

```text
java-backend-academy/
├── 01-api-first/
├── 02-java-spring-boot/
├── 03-clean-architecture/
├── 04-banking-microservices/
├── 05-reactive-quarkus/
├── 06-distributed-systems/
├── 07-azure-devsecops/
├── 08-senior-challenge/
├── shared/
│   ├── contracts/
│   ├── architecture/
│   └── guidelines/
└── README.md
```

---

# 4. Metodología de enseñanza

Cada clase tendrá:

1. **Fundamentos:** explicación teórica.
2. **Ejemplo empresarial:** caso de uso contextualizado.
3. **Live Coding:** demostración del instructor.
4. **Laboratorio:** ejercicio práctico.
5. **Code Review:** revisión de implementación.
6. **Evaluación:** preguntas conceptuales y técnicas.
7. **Documentación:** referencias para profundizar.

## Evaluación por proyecto

| Criterio                        |     Peso |
| ------------------------------- | -------: |
| Fundamentos y conceptos         |      25% |
| Implementación funcional        |      25% |
| Arquitectura y buenas prácticas |      20% |
| Testing y seguridad             |      15% |
| Defensa técnica                 |      15% |
| **Total**                       | **100%** |

Nota mínima sugerida: **80/100**.

---

# 5. Plan de clases — Proyecto 01

## API First & Contract Design

| Clase | Tema                       | Contenido                                         |
| ----- | -------------------------- | ------------------------------------------------- |
| 01    | Fundamentos de APIs        | HTTP, cliente-servidor, REST y SOAP               |
| 02    | Diseño REST                | Recursos, URIs, métodos y códigos HTTP            |
| 03    | API First                  | Contract First vs. Code First                     |
| 04    | OpenAPI básico             | YAML, info, servers, paths y operations           |
| 05    | Modelado de datos          | Schemas, DTOs, tipos y validaciones               |
| 06    | Contratos reutilizables    | Components, $ref, parameters y responses          |
| 07    | Errores empresariales      | Errores funcionales, técnicos y Problem Details   |
| 08    | Seguridad de APIs          | OAuth2, JWT, API Keys y scopes                    |
| 09    | Buenas prácticas bancarias | BIAN, nomenclatura, trazabilidad y versionamiento |
| 10    | Validación de contratos    | Swagger Editor, linters y pruebas contractuales   |
| 11    | Laboratorio integral       | Diseñar Banking Customer API                      |
| 12    | Evaluación y defensa       | Code Review y entrevista técnica                  |

### Entregable final del primer módulo

```text
banking-customer-api/
├── contracts/
│   └── customer-api.yaml
├── docs/
│   ├── api-guidelines.md
│   ├── error-catalog.md
│   ├── requirements.md
│   └── security.md
├── postman/
│   └── customer-api.collection.json
└── README.md
```

### Criterios de aceptación

- El contrato cumple la especificación OpenAPI.
- Los endpoints tienen nombres consistentes.
- Los schemas están correctamente definidos.
- Las respuestas HTTP están documentadas.
- Los errores tienen un formato consistente.
- Se documentan los mecanismos de seguridad.
- Se definen ejemplos de solicitudes y respuestas.
- El contrato puede visualizarse en Swagger Editor.
- El alumno explica y defiende sus decisiones.

---

# 6. Competencias de egreso

Al finalizar, el estudiante deberá poder:

- Diseñar contratos API First.
- Desarrollar APIs Java con Spring Boot.
- Aplicar POO, SOLID y patrones de diseño.
- Implementar arquitectura hexagonal.
- Crear y consumir microservicios.
- Integrar REST, SOAP y bases de datos.
- Implementar autenticación y autorización.
- Desarrollar servicios reactivos.
- Utilizar Quarkus.
- Aplicar patrones de sistemas distribuidos.
- Implementar pruebas automatizadas.
- Configurar pipelines CI/CD.
- Desplegar aplicaciones en Azure.
- Investigar errores y problemas de rendimiento.
- Realizar Code Reviews.
- Defender decisiones arquitectónicas.

---

# 7. Proyecto final integrador

## Banking Platform

Sistema bancario ficticio compuesto por:

- Customer Service.
- Account Service.
- Transfer Service.
- Authentication Service.
- Notification Service.
- Audit Service.
- API Gateway.

### Capacidades

- Gestión de clientes.
- Gestión de cuentas.
- Consulta de saldos.
- Transferencias.
- Autenticación.
- Autorización.
- Auditoría.
- Trazabilidad.
- Integración asíncrona.
- Recuperación ante fallos.
- Monitoreo.

### Requisitos técnicos

- Java 21.
- Spring Boot.
- Arquitectura hexagonal.
- OpenAPI.
- OAuth2/JWT.
- PostgreSQL u Oracle.
- Docker.
- Kubernetes.
- Azure.
- CI/CD.
- JUnit y Mockito.
- Observabilidad.

### Evaluación final

El alumno deberá demostrar el funcionamiento de la plataforma, explicar la arquitectura, justificar sus decisiones técnicas y responder preguntas equivalentes a una entrevista Backend Java Mid/Senior.

---

# 8. Referencias adicionales

## Java

- https://dev.java/
- https://docs.oracle.com/en/java/

## Spring

- https://spring.io/
- https://docs.spring.io/spring-boot/reference/
- https://docs.spring.io/spring-security/reference/

## Arquitectura

- https://martinfowler.com/
- https://c4model.com/
- https://microservices.io/

## APIs

- https://spec.openapis.org/
- https://swagger.io/docs/
- https://bian.org/

## Testing

- https://junit.org/
- https://site.mockito.org/
- https://java.testcontainers.org/

## Cloud y DevOps

- https://learn.microsoft.com/en-us/azure/
- https://learn.microsoft.com/en-us/azure/devops/
- https://kubernetes.io/docs/
- https://docs.docker.com/

## Seguridad

- https://owasp.org/
- https://oauth.net/2/

---

**Java Backend Engineering Academy**

_Programa de formación orientado a ingeniería backend empresarial y bancaria._
