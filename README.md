# Abderaouf Bouzerara

**Backend engineer** · TypeScript · NestJS · PostgreSQL

Four years as a backend engineer. Looking for a remote role.

[LinkedIn](https://linkedin.com/in/rbdz)

## Projects

Three open-source repos that make up one product. The API holds the domain logic, auth, and business rules. The admin dashboard and storefront are clients on top of it. Everything runs locally; there is no hosted demo.

### [E-commerce Store API](https://github.com/raouf-b-dev/ecommerce-store-api)

NestJS modular monolith for catalog, cart, checkout, payments, inventory, and identity. Spin it up with Docker. Payments go through a mock adapter.

- Modules stay independent: they talk through gateways and events instead of importing each other's internals.
- Checkout stays consistent with a compensating BullMQ SAGA. Stock is protected with PostgreSQL row locks.
- Redis speeds up reads and dedupes writes. Auth uses RSA JWT/JWKS, rotating refresh tokens, and RBAC.
- List and detail reads go through CQRS query adapters. CI fails if a module crosses a boundary.
- Jest, Testcontainers, e2e and integration tests, GitHub Actions.
- OpenTelemetry, Prometheus, Grafana, and structured logs.

### [E-commerce Admin Dashboard](https://github.com/raouf-b-dev/ecommerce-admin-dashboard)

React (Vite) operator console for that API: products, categories, inventory, orders, users, and roles.

- UI client is generated from OpenAPI so the screens stay in sync with the API. No BFF.
- Nav and pages filter by permissions for UX; the API still enforces access.
- Point it at a local API, or use MSW when you only need the UI.

### [E-commerce Storefront](https://github.com/raouf-b-dev/ecommerce-store-web)

Next.js App Router customer storefront for the same API: catalog, cart, checkout, orders, and account.

- OpenAPI-typed client. The app handles UI and caching; pricing, stock, and checkout stay in the API.
- Point it at a local API, or use MSW for shopper paths when you only need the UI.

## Stack

**Backend:** TypeScript · Node.js · NestJS · PostgreSQL · TypeORM · Redis · BullMQ  
**Architecture:** DDD · Hexagonal · CQRS · SAGA  
**Security:** RBAC · JWT/JWKS · refresh-token rotation · rate limiting  
**Infra:** Docker · GitHub Actions · Jest · Testcontainers · OpenTelemetry · Prometheus · Grafana  
**Frontend:** React · Next.js · Vite · TanStack Query · Angular · RxJS · NgRx
