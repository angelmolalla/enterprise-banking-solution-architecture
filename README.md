# 🏦 Enterprise Banking Solution Architecture

## Descripción

Este repositorio contiene una propuesta de arquitectura de software para una plataforma de **Banca por Internet (Internet Banking)** desarrollada utilizando el modelo C4 y principios de arquitectura empresarial.

La solución fue diseñada para soportar los principales procesos de una entidad financiera, garantizando escalabilidad, resiliencia operativa, seguridad, alta disponibilidad y cumplimiento de normativa bancaria y de protección de datos.

---

# Contenido del repositorio

El repositorio contiene la documentación técnica y los diagramas utilizados para el diseño de la solución.

```
📂 docs
 ├── Documento de Arquitectura.pdf
 ├── Diagrama C1 - Contexto
 ├── Diagrama C2 - Contenedores
 ├── Diagramas C3 - Componentes
 ├── Diagramas de Secuencia
 ├── Diagrama de Infraestructura
 └── Estimación de Costos

📂 diagrams
 ├── C1
 ├── C2
 ├── C3
 ├── Infrastructure
 └── Sequence
```

---

# Objetivo

Diseñar una arquitectura de software para una plataforma de banca digital que permita:

- Registro de clientes.
- Consulta de movimientos.
- Pagos internos.
- Pagos interbancarios.
- Gestión de consentimiento de datos.
- Auditoría de operaciones.
- Envío de notificaciones.

Todo ello garantizando:

- Alta disponibilidad.
- Escalabilidad horizontal.
- Seguridad.
- Resiliencia.
- Cumplimiento normativo.

---

# Arquitectura

La solución adopta una arquitectura distribuida basada en microservicios desplegada sobre Kubernetes.

Cada dominio funcional mantiene independencia de datos y de despliegue, favoreciendo el desacoplamiento y la evolución independiente de los servicios.

---

# Patrones arquitectónicos implementados

- API Gateway
- Microservicios
- CQRS
- Saga Orquestada
- Outbox Pattern
- Circuit Breaker
- Cache Aside
- Arquitectura Orientada a Eventos (Event-Driven Architecture)

---

# Tecnologías utilizadas

## Backend

- Java
- Spring Boot
- Spring Security
- REST APIs

## Frontend

- Angular
- React Native

## Infraestructura

- Docker
- Kubernetes
- NGINX
- WAF

## Persistencia

- Microsoft SQL Server
- MongoDB
- Redis

## Integración

- Apache Kafka
- API Gateway

## Seguridad

- OAuth 2.0
- Microsoft Entra ID
- JWT
- TLS

## Observabilidad

- Logs
- Métricas
- Monitoreo
- Auditoría

---

# Principios arquitectónicos

La solución fue diseñada bajo los siguientes principios:

- Zero Trust.
- Seguridad por diseño.
- Protección de datos por defecto.
- Alta disponibilidad.
- Escalabilidad horizontal.
- Resiliencia operativa.
- Desacoplamiento funcional.

---

# Cumplimiento normativo

La propuesta considera normativa y estándares relacionados con:

- Libro de Normas de Control para las Entidades de los Sectores Financieros Público y Privado.
- Ley Orgánica de Protección de Datos Personales (LOPDP).
- Guía de Protección de Datos Personales desde el Diseño y por Defecto.
- ISO 27001.
- ISO 27017.
- ISO 27018.

---

# Diagramas incluidos

El proyecto incorpora los siguientes diagramas:

- Modelo C4
  - Contexto (C1)
  - Contenedores (C2)
  - Componentes (C3)

- Diagramas de Secuencia
  - Onboarding
  - Pago Interno
  - Pago Interbancario
  - Consulta de Movimientos

- Diagrama de Infraestructura

---

# Infraestructura

La infraestructura contempla:

- Kubernetes
- Alta disponibilidad
- Balanceadores
- Autoescalado (HPA)
- Bases de datos distribuidas
- Mensajería mediante Kafka
- Observabilidad
- Recuperación ante fallos

También se incluye una estimación referencial de recursos de infraestructura y costos operativos.

---

# Autor

**Marcelo Olalla**

Ingeniero en Sistemas

Arquitecto de Soluciones