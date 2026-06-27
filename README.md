# Smart Waste Collection System

A full-stack IoT-powered waste management platform for municipalities.

## Stack

| Layer | Technology |
|---|---|
| Frontend | React 18 + TypeScript + Tailwind CSS + Vite |
| Backend | FastAPI (Python 3.11) |
| Database | PostgreSQL 15 + SQLAlchemy |
| Cache | Redis 7 |
| Message Queue | AWS SQS |
| IoT | AWS IoT Core → Lambda |
| Deployment | Docker + AWS ECS Fargate |
| CI/CD | GitHub Actions |

## Quick start

```bash
git clone https://github.com/your-org/smart-waste-system.git
cd smart-waste-system
cp .env.example .env
docker-compose up --build
```

- Frontend: http://localhost:3000
- Backend API: http://localhost:8000
- API Docs: http://localhost:8000/docs
- PgAdmin: http://localhost:5050

## Project structure

```
smart-waste-system/
├── frontend/          React dashboard + citizen app
├── backend/           FastAPI REST API
├── database/          Migrations + seeds
├── docker/            Dockerfiles
├── infrastructure/    AWS CDK + Kubernetes manifests
├── scripts/           Dev utilities
└── .github/workflows/ CI/CD pipelines
```

## Modules

1. **Real-time dashboard** — live bin map, alerts, analytics
2. **Collection team app** — route, tasks, mark-as-collected
3. **Citizen complaint module** — report, photo upload, tracking
4. **Route optimization** — VRP/Dijkstra/A*/Genetic algorithms
5. **IoT sensor pipeline** — ESP32 → AWS IoT Core → API
6. **AI predictions** — overflow forecasting with LSTM/XGBoost
