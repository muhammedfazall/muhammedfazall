# Muhammed Fazal

Backend engineer building Go systems

[GitHub](https://github.com/muhammedfazall) · [LinkedIn](https://www.linkedin.com/in/muhammedfazall/) · [Email](mailto:fazalbkabeer@gmail.com)

## Now

Building MoneyMate, a personal finance platform split into Go microservices communicating over gRPC with shared protobuf contracts, backed by Postgres, Redis, and Kafka. Current focus: RBAC across services, Argon2 password hashing, Redis-backed token management, and the Kafka consumer layer.

Repo: [moneymate-2026/moneymate-backend](https://github.com/moneymate-2026/moneymate-backend)

## Sendr

Transactional email platform with a CLI client, running in production.

```
        React UI            Sendr CLI
             \                 /
                  Go API
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
   PostgreSQL     Redis      Razorpay
        │
   Job Queue → Worker Pool → SendGrid
```

Job queue, implemented in Postgres:

```sql
SELECT * FROM jobs
WHERE status = 'pending'
ORDER BY created_at
FOR UPDATE SKIP LOCKED
LIMIT 10;
```

A semaphore-bounded worker pool claims rows with that query, retries failures with exponential backoff, and moves jobs that fail repeatedly to a dead letter queue with zombie-job recovery. Delivery goes through SendGrid; Sendr handles orchestration.

Also included:
- Hexagonal architecture: domain, ports, adapters, dependency injection
- Google OAuth and RS256 JWTs with refresh rotation and Redis-backed blacklisting
- API keys hashed with SHA-256, compared in constant time
- Per-user rate limiting via atomic Lua scripts in Redis
- Idempotent Razorpay billing: subscriptions, webhook verification, plan-based access
- Cobra + GoReleaser CLI for login, API key management, sending mail, and delivery status
- Deployed to EC2 via GitHub Actions

Stack: Go, Chi, PostgreSQL, Redis, Docker, AWS, Razorpay
Code: [muhammedfazall/Sendr](https://github.com/muhammedfazall/Sendr)

The React dashboard shown above uses this same Go API.

## SneaCave

E-commerce backend: row-level locking on checkout, transactional order placement, OTP-verified auth with Redis-backed refresh tokens, admin dashboard with Chart.js analytics.

Stack: Go, Gin, GORM, PostgreSQL, Redis, Docker
Code: [muhammedfazall/go-ecommerce](https://github.com/muhammedfazall/go-ecommerce)

## Stack, generally

Go · gRPC · REST · PostgreSQL (SQLC, GORM) · Redis · Kafka · Fiber / Gin / Chi · Docker · AWS EC2 · GitHub Actions · React

## Also

Distributed systems, database internals, algorithms.

---

Open to backend engineering roles.
