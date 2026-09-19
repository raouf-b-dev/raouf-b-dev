# Abderaouf Bouzerara

**Backend engineer** · TypeScript · NestJS · PostgreSQL

Four years as a backend engineer. Looking for a remote role.

[LinkedIn](https://linkedin.com/in/rbdz)

## Projects

Three open-source repos, one product. The API owns domain logic, auth, and business rules. The admin dashboard and storefront are React/Next clients on top of it. Run locally — no hosted demo.

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

### [E-commerce Storefront](https://github.com/raouf-b-dev/ecommerce-store-web)

Next.js App Router customer storefront for the same API: catalog, cart, checkout, orders, and account.

- OpenAPI-typed client; UI and caching only — pricing, stock, and checkout stay in the API.
- Run against a local API, or MSW for shopper paths when you only need the UI.

## Stack

**Backend:** TypeScript · Node.js · NestJS · PostgreSQL · TypeORM · Redis · BullMQ  
**Architecture:** DDD · Hexagonal · CQRS · SAGA  
**Security:** RBAC · JWT/JWKS · refresh-token rotation · rate limiting  
**Infra:** Docker · GitHub Actions · Jest · Testcontainers · OpenTelemetry · Prometheus · Grafana  
**Frontend:** React · Next.js · Vite · TanStack Query · Angular · RxJS · NgRx
