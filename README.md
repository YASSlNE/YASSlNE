# Mahmoud Yassine Chiboub

Hi, I’m Mahmoud 👋  
I’m a backend-focused software engineer with experience building and operating production systems, APIs, and real-time services.

I’ve worked on cloud-native applications in health-tech and SaaS environments, focusing on reliability, maintainability, and clean deployments.

## What I work on
- Backend APIs and real-time systems
- Async processing and system reliability
- Cloud deployments with Docker and CI/CD
- Frontend development (React / Next.js) for API-driven applications

## Featured Projects

### 🔹 Real-Time Customer Operations Platform
Backend system powering a customer service and operations web application with real-time interactions.

- Designed and maintained REST APIs supporting orders, recurring orders, and customer workflows
- Implemented real-time messaging and notifications using WebSockets with MongoDB
- Integrated frontend (React / Next.js) with backend services for live updates
- Worked on dashboards and internal tools for operational visibility
- Containerized services and supported frequent deployments using Docker and CI/CD pipelines



### 🔹 Async Job Processing System 

A production-style backend that handles long-running tasks asynchronously using a queue + worker architecture.

This project is designed to demonstrate real-world backend/system patterns: async processing, retries, idempotency, failure handling, and AWS-ready deployment.

---

#### Why this exists
Many real applications must process work that cannot finish within a typical HTTP request:
- AI/LLM tasks (summarization, embeddings)
- report generation
- PDF/image processing
- bulk imports/exports
- webhook fan-out

The API should respond immediately, while background workers execute the job reliably.

---

## Core Features
- **Async architecture**: API → Queue → Worker
- **Job lifecycle**: `QUEUED` → `RUNNING` → `SUCCEEDED` / `FAILED_FINAL`
- **Retries & failure handling**:
  - retryable vs non-retryable error classification
  - max attempts + DLQ (Dead Letter Queue)
- **Idempotency**:
  - safe `POST /jobs` with an `idempotencyKey` to prevent duplicates
- **Job status tracking**:
  - poll status via `GET /jobs/{id}`
- **Dockerized services**
- **AWS-ready deployment** (SQS + RDS + ECS/EC2)

## Technical Focus

**Backend & APIs**
- Go, Python (FastAPI), TypeScript
- REST APIs, background workers, WebSockets

**Cloud & DevOps**
- AWS (EC2, Elastic Beanstalk)
- Docker, CI/CD with GitHub Actions
- Basic system design and scalability concepts

**Databases**
- PostgreSQL, MySQL, MongoDB
- Schema design and data consistency

## Experience Snapshot
- Software Engineer at Avey (Health-Tech / EMR systems)
- Backend Developer at Synque (APIs, real-time platforms, CI/CD)
- Experience working in production and remote environments

📬 Open to remote freelance or contract work  
📎 LinkedIn: https://www.linkedin.com/in/mahmoud-yassine-chiboub  
📧 Email: mdyassinechiboub@gmail.com
