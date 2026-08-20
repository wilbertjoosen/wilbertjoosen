# Wilbert Joosen

**Senior Software Engineer · Software Architect · Technical Lead**

Brasília, Brazil

I design and build distributed systems end to end — service boundaries, event-driven
communication, and the delivery pipeline that gets them into production safely. My focus is
backend architecture in Java/Spring, with the surrounding Kubernetes/GitOps tooling that makes a
microservices system operable rather than just runnable.

## Focus areas

- Microservices architecture and distributed-systems patterns — sagas, CQRS, circuit breakers,
  outbox, event-driven design
- Java / Spring Boot, Kafka
- Kubernetes, GitOps (ArgoCD), Docker
- Identity and access management — Keycloak, OAuth2/OIDC
- Technical leadership — architecture decisions grounded in *why* a pattern is needed, not just
  how to wire it up

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
