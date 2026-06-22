# Enterprise System 20260622 224615 Qhg2Fj99Rq8L

![Build](https://github.com/efealtiparmakoglu/enterprise-system-20260622-224615-qhg2fj99rq8l/workflows/CI%20Pipeline/badge.svg)
![Python](https://img.shields.io/badge/python-3.11-blue)
![License](https://img.shields.io/badge/license-MIT-green)

Enterprise-grade microservice architecture with FastAPI, PostgreSQL, Redis, and Kubernetes.

## 🏗️ Architecture

```
┌──────────┐      ┌──────────┐      ┌──────────┐
│  Nginx   │──────▶│ FastAPI  │──────▶│   DB     │
│ (Load    │      │ (App)    │      │(PostgreSQL)│
│  Balancer)│     └────┬─────┘      └──────────┘
└──────────┘          │
                      ▼
               ┌──────────┐
               │  Redis   │
               │ (Cache)  │
               └──────────┘
```

## 🚀 Features

- **FastAPI** - Modern async web framework
- **PostgreSQL** - Robust database with SQLAlchemy ORM
- **Redis** - High-performance caching layer
- **Docker** - Containerization with Compose
- **Kubernetes** - Production orchestration
- **CI/CD** - GitHub Actions pipelines
- **Testing** - pytest with coverage
- **Migrations** - Alembic database migrations

## 📦 Installation

```bash
# Clone
git clone https://github.com/efealtiparmakoglu/enterprise-system-20260622-224615-qhg2fj99rq8l.git
cd enterprise-system-20260622-224615-qhg2fj99rq8l

# Install
make install

# Run locally
make run
```

## 🐳 Docker

```bash
# Start all services
docker-compose up -d

# View logs
docker-compose logs -f app
```

## ☸️ Kubernetes

```bash
# Deploy to cluster
kubectl apply -f k8s/

# Check status
kubectl get pods -n enterprise-system-20260622-224615-qhg2fj99rq8l
```

## 🧪 Testing

```bash
make test
```

## 📝 API Documentation

- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc
- Health: http://localhost:8000/health

## License

MIT License - see LICENSE file
