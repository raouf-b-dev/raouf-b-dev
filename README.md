# Abderaouf Bouzerara

**Backend engineer**

4 years of professional experience building APIs. Looking for a remote role.

[LinkedIn](https://linkedin.com/in/rbdz)

## Projects

One open-source ecommerce product across four repos. The API owns the domain and the OpenAPI contract. Admin and storefront are clients generated from that contract. Platform is a Docker Compose setup that runs the pinned images.

Hosted demo coming soon, or run it locally with Compose.

### [E-commerce Store API](https://github.com/raouf-b-dev/ecommerce-store-api)

NestJS modular monolith for catalog, cart, checkout, payments, inventory, and identity. Payments use a stubbed Stripe provider behind a port.

### [E-commerce Admin Dashboard](https://github.com/raouf-b-dev/ecommerce-admin-dashboard)

Vite + React operator console for that API. OpenAPI-generated client; no BFF.

### [E-commerce Storefront](https://github.com/raouf-b-dev/ecommerce-store-web)

Next.js App Router shopper app for the same API. OpenAPI-typed client; pricing, stock, and checkout stay in the API.

### [E-commerce Platform](https://github.com/raouf-b-dev/ecommerce-platform)

Compose only. Pulls versioned images for the API, admin, storefront, Postgres, and Redis.

## Stack

**Backend:** TypeScript · Node.js · NestJS · PostgreSQL · TypeORM · Redis · BullMQ · OpenAPI  
**Ship:** Docker · GitHub Actions · Jest · Testcontainers  
**Clients:** React · Next.js · Vite · Angular · RxJS · NgRx
