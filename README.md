# 🐳 Mini Microservices Architecture with Docker Compose

A fully containerized microservices architecture using **Docker Compose** — featuring a React frontend, Node.js backend, PostgreSQL, MongoDB, Redis, RabbitMQ, and NGINX as a reverse proxy.

> Built to simulate real-world DevOps-ready service orchestration locally.

---

## 🚀 Project Overview

This project showcases a **modular microservices stack** wired together with Docker Compose, demonstrating real-world development patterns like:

- Multi-service container orchestration
- Database integration (SQL & NoSQL)
- Caching & pub/sub mechanisms
- Frontend-backend API routing via NGINX
- Local emulation of production infrastructure

---

## 🧱 Tech Stack

| Service     | Tech              | Description                                |
|-------------|-------------------|--------------------------------------------|
| `frontend`  | React.js          | SPA built and served from container        |
| `backend`   | Node.js + Express | REST API exposing endpoints for frontend   |
| `postgres`  | PostgreSQL        | Relational DB for structured data          |
| `mongodb`   | MongoDB           | NoSQL DB for unstructured data             |
| `redis`     | Redis             | In-memory caching                          |
| `rabbitmq`  | RabbitMQ          | Message broker for inter-service comms     |
| `nginx`     | NGINX             | Reverse proxy and static file routing      |

---

## 📁 Directory Structure

mini-microservices/
├── backend/ # Node.js Express backend
│ └── Dockerfile
├── frontend/ # React frontend
│ └── Dockerfile
├── nginx/ # NGINX configuration
│ └── default.conf
├── docker-compose.yml # Docker Compose orchestration
└── .env # Environment variable definitions

text

---

## ⚙️ Features

- 🐳 **Multi-container orchestration** using Docker Compose
- 🔁 **Service-to-service networking** via internal Docker bridge
- 🔗 **NGINX reverse proxy** with routing to `/api` and `/`
- 💾 **PostgreSQL & MongoDB** databases integrated into backend
- 🧠 **Redis caching** enabled
- 🐇 **RabbitMQ queue** wired for future async messaging
- 🎯 **Separation of concerns**: each service has its own Dockerfile and config

---

## 🧠 Why Docker Compose?

While many stop at learning basic Docker commands, real deployments involve **many services working together**.

Docker Compose allows:
- Declarative configuration of the entire stack
- Easy service scaling
- Centralized `.env` variable management
- Local simulation of production architecture
- The **perfect bridge** to learning Kubernetes

---

## ✅ Getting Started

1. **Clone the repo**
git clone https://github.com/your-username/mini-microservices.git
cd mini-microservices

text

2. **Start the services**
docker-compose up --build

text

---

### Access Services

- **Frontend:** http://localhost:80
- **Backend API:** http://localhost/api
- **RabbitMQ Dashboard:** http://localhost:15672 (guest/guest)
- **PostgreSQL:** port 5432
- **MongoDB:** port 27017

---

### 📦 Environment Variables

Configure your `.env` file:

POSTGRES_USER=devuser
POSTGRES_PASSWORD=devpass
POSTGRES_DB=mydb
MONGO_INITDB_DATABASE=mydb
REDIS_PORT=6379

text

---

### 🧪 Testing the Setup

- Use `docker ps` to verify all services are running
- Check frontend API integration
- Access RabbitMQ dashboard to inspect queues
- Monitor logs using `docker-compose logs -f`

---

## 🛠️ Future Enhancements

- Docker Swarm / Kubernetes (EKS) deployment
- CI/CD automation with Jenkins or GitHub Actions
- NGINX rate limiting, HTTPS
- Prometheus + Grafana for container monitoring
- Microservice auth gateway (e.g., JWT or OAuth2)

---

## 🤝 Let's Connect

Feel free to reach out if you're working on:

- DevOps + Docker Projects
- Microservices / Distributed Systems
- Fullstack Infra-as-Code deployments
- Open to internships, collaborations, and freelance gigs 🚀

---

## 🔗 License

MIT License. Use freely and contribute back if you'd like!

---

## 💬 Feedback & Contributions Welcome!

If you found this useful, give it a ⭐ on GitHub.  
Feel free to open issues or PRs for improvemen
