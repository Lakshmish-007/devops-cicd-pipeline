# CI/CD Pipeline with Docker and GitHub Actions

Automated CI/CD pipeline that builds and pushes a Docker image to DockerHub on every GitHub push. No manual steps are involved.

---

## What it does

Every time code is pushed to the main branch, GitHub Actions automatically:

1. Pulls the latest code
2. Builds a Docker image
3. Pushes the image to DockerHub

---

## Tech Stack

- Docker
- GitHub Actions
- Node.js
- DockerHub

---

## Project Structure
```
devops-cicd-pipeline/
├── .github/
│   └── workflows/
│       └── ci.yml        # GitHub Actions pipeline
├── Dockerfile            # Docker image config
├── index.js              # Node.js app
└── package.json          # Dependencies
```

---

## How it works

The GitHub Actions workflow is defined in `.github/workflows/ci.yml`. It triggers on every push to main, builds the Docker image using the Dockerfile, and pushes it to DockerHub automatically.

---

