# Abderaouf Bouzerara

**Backend engineer** · TypeScript · NestJS · PostgreSQL

Four years as a backend engineer. Looking for a remote role.

[LinkedIn](https://linkedin.com/in/rbdz)

## Projects

The store API and the admin dashboard are one product. The API holds domain logic, auth, and business rules. The dashboard is a React client on top of it.

### [E-commerce Store API](https://github.com/raouf-b-dev/ecommerce-store-api)

NestJS modular monolith covering catalog, cart, checkout, payments, inventory, and identity. Reference backend: run it locally with Docker. Payments use a mock adapter.

- Keep modules independent by talking through gateways and events instead of importing internals.
- Keep checkout consistent with a compensating BullMQ SAGA. Protect stock with PostgreSQL row locks.
- Speed up reads and dedupe writes with Redis. Authenticate with RSA JWT/JWKS, rotating refresh tokens, and RBAC.
- Separate list/detail reads with CQRS query adapters. Fail CI when a module crosses a boundary.
- Jest, Testcontainers, e2e and integration tests, GitHub Actions.
- OpenTelemetry, Prometheus, Grafana, and structured logs.

### [E-commerce Admin Dashboard](https://github.com/raouf-b-dev/ecommerce-admin-dashboard)

React (Vite) operator console for that API: products, categories, inventory, orders, users, and roles.

- Generate the UI client from OpenAPI so screens stay aligned with the API. No BFF.
- Filter nav and pages by permissions for UX. Enforce access on the API.
- Run against a local API, or MSW when you only need the UI.

## Stack

**Backend:** TypeScript · Node.js · NestJS · PostgreSQL · TypeORM · Redis · BullMQ  
**Architecture:** DDD · Hexagonal · CQRS · SAGA  
**Security:** RBAC · JWT/JWKS · refresh-token rotation · rate limiting  
**Infra:** Docker · GitHub Actions · Jest · Testcontainers · OpenTelemetry · Prometheus · Grafana  
**Frontend:** Angular · RxJS · NgRx · React · TanStack Query
