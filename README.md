<div align="center">

# Muhammed Fazal

### Backend Engineer · Go · Microservices · Distributed Systems

**Building reliable backend systems with Go, PostgreSQL, Redis, gRPC & AWS**

<p>
  <a href="https://github.com/muhammedfazall">
    <img src="https://img.shields.io/badge/GitHub-muhammedfazall-181717?style=for-the-badge&logo=github" />
  </a>
  <a href="https://www.linkedin.com/in/muhammedfazall/">
    <img src="https://img.shields.io/badge/LinkedIn-Muhammed%20Fazal-0A66C2?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="mailto:fazalbkabeer@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

</div>

---

## About Me

I'm a **Backend Engineer specializing in Go**, with hands-on experience designing and building backend systems, REST APIs, microservices, and asynchronous processing workflows.

My focus is on building systems that are:

* **Clean** — well-structured architecture and separation of concerns
* **Reliable** — retries, failure recovery, idempotency, and transactional consistency
* **Performant** — concurrency, efficient database access, caching, and rate limiting
* **Maintainable** — clear interfaces, modular services, and production-oriented workflows

I'm particularly interested in **backend architecture, distributed systems, concurrency, databases, and system design**.

---

## 🔭 Currently Working On

### MoneyMate — Personal Finance Platform

A Go-based **microservices platform** for personal finance management.

```text
API Gateway
     │
     ├──────────────┐
     ▼              ▼
 Auth Service   Merchant Service
     │              │
     └──────┬───────┘
            ▼
       PostgreSQL
            │
          Redis
            │
          Kafka
```

**Working with:**

`Go` · `Fiber` · `gRPC` · `PostgreSQL` · `Redis` · `SQLC` · `Kafka` · `Docker`

Current focus:

* Microservices architecture
* gRPC service-to-service communication
* Shared protobuf contracts
* Authentication & RBAC
* PostgreSQL schema design
* Redis-backed token management
* Kafka-based asynchronous communication
* Containerized services

---

# 🚀 Featured Projects

## 01 · Sendr

### Transactional Email Platform & Developer CLI

A developer-facing email delivery platform built with Go, designed around **asynchronous processing, clean architecture, reliability, and secure API access**.

### Architecture

```text
                     ┌──────────────┐
                     │   React UI   │
                     └──────┬───────┘
                            │
                            ▼
┌──────────────┐     ┌──────────────┐
│  Sendr CLI   │────▶│   Go API     │
└──────────────┘     └──────┬───────┘
                            │
              ┌─────────────┼──────────────┐
              ▼             ▼              ▼
         PostgreSQL       Redis         Razorpay
              │
              ▼
        Job Queue
              │
              ▼
       Worker Pool
              │
              ▼
          SendGrid
```

### Engineering Highlights

**Architecture**

* Hexagonal / Clean Architecture
* Domain, ports, and adapters separation
* Dependency injection
* Modular service design

**Job Processing**

* PostgreSQL-backed job queue
* `SELECT FOR UPDATE SKIP LOCKED`
* Semaphore-bounded worker pool
* Concurrent job processing
* Exponential backoff
* Retry handling
* Dead Letter Queue
* Zombie job recovery

**Security**

* Google OAuth
* RS256 JWT authentication
* Refresh token rotation
* Redis-backed token blacklisting
* API key authentication
* SHA-256 API key hashing
* Constant-time credential comparison

**Reliability & Performance**

* Redis-backed rate limiting
* Atomic Lua scripts
* Per-user usage limits
* Idempotent payment processing
* Transactional database workflows

**Payments**

* Razorpay integration
* Subscription plans
* Payment verification
* Webhook handling
* Plan-based access control

**Infrastructure**

* Docker
* GitHub Actions
* GoReleaser
* AWS EC2
* SendGrid

**Stack**

`Go` `Chi` `PostgreSQL` `Redis` `Docker` `AWS` `SendGrid` `Razorpay` `GitHub Actions`

---

## 02 · MoneyMate

### Personal Finance Platform · Ongoing

A Go-based microservices platform focused on personal finance management.

### Engineering Highlights

* Microservices architecture
* API Gateway
* gRPC service communication
* Shared protobuf contracts
* PostgreSQL with SQLC
* Goose migrations
* Redis-backed authentication infrastructure
* JWT & refresh tokens
* RBAC
* Argon2 password hashing
* Kafka-based asynchronous communication
* Dockerized services

**Stack**

`Go` `Fiber` `gRPC` `PostgreSQL` `Redis` `SQLC` `Kafka` `Docker`

---

## 03 · SneaCave

### E-Commerce Platform

A full-featured e-commerce platform with transactional order processing and a server-rendered administration system.

### Features

**Customer**

* Product catalog
* Cart management
* Wishlist
* Order management
* Authentication

**Business Logic**

* Transactional order placement
* Inventory validation
* Row-level locking
* Database consistency

**Authentication**

* JWT
* Redis refresh-token storage
* Token blacklisting
* OTP email verification
* Role-based authorization

**Administration**

* Product management
* Category management
* User management
* Order management
* Dashboard analytics
* Chart.js visualizations

**Infrastructure**

* Docker
* Docker Compose
* GitHub Actions

**Stack**

`Go` `Gin` `GORM` `PostgreSQL` `Redis` `Docker`

---

## 04 · Sendr CLI

### Developer Command-Line Client

A cross-platform CLI for interacting with the Sendr platform.

### Features

* Browser-based OAuth login
* API key management
* Email sending from terminal
* Local configuration management
* Delivery status polling
* Cross-platform builds
* Automated releases

**Stack**

`Go` `Cobra` `GoReleaser` `GitHub Actions`

---

# 🧠 Engineering Interests

<div align="center">

|   Backend  |        Systems       | Infrastructure |
| :--------: | :------------------: | :------------: |
|     Go     |  Distributed Systems |       AWS      |
|  REST APIs |     Microservices    |     Docker     |
|    gRPC    |      Concurrency     |      CI/CD     |
| PostgreSQL | Event-Driven Systems |      Linux     |
|    Redis   |     System Design    | GitHub Actions |

</div>

---

# 🛠️ Tech Stack

### Languages

<p>
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
</p>

### Backend

<p>
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white"/>
<img src="https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=google&logoColor=white"/>
<img src="https://img.shields.io/badge/REST%20API-005571?style=flat-square"/>
<img src="https://img.shields.io/badge/Microservices-FF6F00?style=flat-square"/>
<img src="https://img.shields.io/badge/Gin-008ECF?style=flat-square"/>
<img src="https://img.shields.io/badge/Fiber-00ADD8?style=flat-square"/>
<img src="https://img.shields.io/badge/Chi-000000?style=flat-square"/>
</p>

### Databases

<p>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLC-000000?style=flat-square"/>
<img src="https://img.shields.io/badge/GORM-00ADD8?style=flat-square"/>
</p>

### Distributed Systems

<p>
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/Job%20Queues-444444?style=flat-square"/>
<img src="https://img.shields.io/badge/Workers-444444?style=flat-square"/>
<img src="https://img.shields.io/badge/Retries-444444?style=flat-square"/>
<img src="https://img.shields.io/badge/DLQ-444444?style=flat-square"/>
<img src="https://img.shields.io/badge/Rate%20Limiting-444444?style=flat-square"/>
</p>

### Authentication & Security

<p>
<img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white"/>
<img src="https://img.shields.io/badge/OAuth%202.0-3C873A?style=flat-square"/>
<img src="https://img.shields.io/badge/RBAC-444444?style=flat-square"/>
<img src="https://img.shields.io/badge/API%20Keys-444444?style=flat-square"/>
</p>

### DevOps & Cloud

<p>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonaws&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
</p>

---

# 📚 Currently Learning

```text
Advanced Go
     │
     ├── Concurrency
     ├── Performance
     └── Production Patterns
     
Distributed Systems
     │
     ├── Microservices
     ├── Kafka
     ├── Event-Driven Architecture
     └── Reliability Patterns

Infrastructure
     │
     ├── AWS
     ├── Observability
     └── Scalable Deployments
```

---

# 🤝 Looking to Collaborate On

* Go backend projects
* Distributed systems
* Microservices
* Open-source Go projects
* Developer tooling
* Infrastructure projects
* Backend-heavy applications

---

# 💬 Ask Me About

**Go · PostgreSQL · Redis · gRPC · REST APIs · Microservices · Docker · Authentication · Backend Architecture · Distributed Systems**

---

# 🧩 Problem Solving

I also spend time strengthening my fundamentals through:

* Data Structures & Algorithms
* LeetCode
* SQL problem solving
* Go implementations of common data structures
* Backend system design

---

# 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=muhammedfazall&show_icons=true&hide_border=true&count_private=true&theme=transparent" height="165"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=muhammedfazall&layout=compact&hide_border=true&theme=transparent" height="165"/>

</div>

---

<div align="center">

### Building backend systems. Learning distributed systems. Getting better every day.

**Open to Backend Engineering opportunities**

</div>
