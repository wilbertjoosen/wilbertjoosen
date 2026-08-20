# Wilbert Joosen

**Senior Software Engineer · Software Architect · Technical Lead**

Brasília, Brazil

20+ years designing, building, and scaling mission-critical systems across public sector,
financial services, healthcare, life sciences, and enterprise environments — backend architecture
in Java (Spring Boot, Quarkus) and PHP (Laravel, Lumen), distributed systems, cloud
infrastructure, and the CI/CD/GitOps pipelines that get them into production safely.

## Technical skills

- **Backend**: Java, Spring Boot, Quarkus, PHP, Laravel, Lumen, Zend Framework
- **Frontend**: TypeScript, Vue.js, React, Angular
- **Architecture**: Microservices, distributed systems, Clean Architecture, Domain-Driven Design,
  design patterns, API design, system modernization
- **Cloud & DevOps**: AWS, Docker, Kubernetes, CI/CD, Jenkins, GitLab CI, ArgoCD, GitHub Actions
- **Messaging & distributed processing**: Apache Kafka, RabbitMQ, Apache Spark, Apache Hadoop
- **Databases**: PostgreSQL, MySQL, Oracle, MongoDB, SQL Server
- **Security & quality**: Keycloak, SSO, OAuth 2.0, SonarQube, automated testing, JMeter, Selenium

## Featured work

### [demo](https://github.com/wilbertjoosen/demo) — Microservices reference architecture

A from-scratch rebuild of a Spring Boot monolith into a 17-service distributed system, built as a
hands-on reference for why you'd reach for a given pattern, not just how to implement it.

- Choreographed Kafka saga (`order → payment → shipping → delivery`) with compensation on failure
- CQRS on the order service (MySQL write model, MongoDB read model); Resilience4j circuit breaker
  on the one synchronous inter-service call in the system
- Full GitOps delivery pipeline — GitHub Actions builds and pushes to GHCR, ArgoCD syncs
  Kubernetes, with a build-once/promote-many flow from a QA namespace to production
- Keycloak (OAuth2/OIDC) across 17 services and a Vue 3 frontend; observability via
  Prometheus/Grafana, Loki, and an audit trail with field-level change history in Kibana

### [keycloak-php](https://github.com/wilbertjoosen/keycloak-php) — Keycloak provider for Laravel/Lumen

A service provider for consuming the Keycloak API and providing authorization in Laravel/Lumen
applications. 9 stars, 4 forks.

## Connect

[LinkedIn](https://linkedin.com/in/wilbertjoosen)
