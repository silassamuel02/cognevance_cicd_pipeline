
# Cognevance CI/CD Pipeline Automation

A Node.js sample application demonstrating automated testing and Docker image building using GitHub Actions.

## Features

- Express.js REST API
- Health-check endpoint
- Automated tests using Jest and Supertest
- Docker containerization
- GitHub Actions CI pipeline

## Requirements

- Node.js 22 or later
- npm
- Docker Desktop (for local container builds)

## Run locally

```bash
npm ci
npm start
```

Visit `http://localhost:3000/` or `http://localhost:3000/health`.

## Run tests

```bash
npm test
```

## Build the Docker image

```bash
docker build -t cognevance-cicd-app .
```

## CI workflow

The workflow in `.github/workflows/ci-cd.yml` runs on pushes and pull requests targeting `main`. It installs dependencies, executes tests, and builds the Docker image.
