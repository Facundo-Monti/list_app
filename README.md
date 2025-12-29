# Lista App

Full-stack task list application with sharing capabilities.

## Tech Stack

- **Frontend:** Angular 17+ with TypeScript
- **Backend:** NestJS with TypeScript
- **Database:** PostgreSQL 16
- **Cache:** Redis
- **DevOps:** Docker, GitHub Actions, Nginx
- **Monitoring:** Sentry, Prometheus, Grafana

## Features

- Create, read, update, and delete lists
- Add items to lists with completion tracking
- Three visibility levels: Public, Shared, Private
- Share lists with specific users
- User authentication and authorization
- Real-time updates
- Responsive design

## Project Structure
```
lista-app/
├── backend/          # NestJS API
├── frontend/         # Angular application
├── infrastructure/   # Docker, configs, monitoring
└── docs/            # Documentation
```

## Prerequisites

- Node.js 20+
- Docker & Docker Compose
- PostgreSQL 16 (if running locally)
- Git

## Quick Start

### Development with Docker
```bash
# Clone the repository
git clone https://github.com/Montusa/list_app.git
cd lista-app

# Copy environment files
cp .env.example .env

# Start all services
docker-compose up -d

# Access the application
# Frontend: http://localhost:4200
# Backend API: http://localhost:3000
# API Docs: http://localhost:3000/api
```

### Local Development
```bash
# Install dependencies
npm install

# Start backend
cd backend
npm run start:dev

# Start frontend (in another terminal)
cd frontend
npm start
```

## Documentation

- [Architecture Overview](docs/architecture/architecture.md)
- [API Documentation](docs/api/openapi.yaml)
- [Database Schema](docs/architecture/database-schema.md)
- [Deployment Guide](docs/deployment/deployment-guide.md)

## Testing
```bash
# Run all tests
npm test

# Backend tests
cd backend
npm run test
npm run test:e2e

# Frontend tests
cd frontend
npm test
npm run e2e
```

## Security

- JWT-based authentication
- Password hashing with bcrypt
- CORS configuration
- Rate limiting
- Input validation and sanitization

## Contact

Project Link: [https://github.com/Montusa/list_app](https://github.com/Montusa/list_app)