# render-ci-cd-pipeline-github

# 🛠️ MLOps: CI/CD Pipeline with GitHub Actions and Render

This repository demonstrates a simple Continuous Integration and Continuous Deployment (CI/CD) pipeline using:

- 🐳 Docker
- 🧪 GitHub Actions for CI
- 🚀 Render Deploy Hook for CD

---

## 📦 What’s Included

| Component | Description |
|-----------|-------------|
| `docker-build-push.yml` | CI workflow: builds Docker image and pushes to Docker Hub |
| `render-cd.yml` | CD workflow: triggers Render deployment on push |
| `Dockerfile` | Containerizes the ML app (Streamlit/FastAPI) |
| `app.py` | Sample ML app |
| `.env.example` | Template for environment variables |

---

## 🔧 GitHub Secrets Needed

| Secret Name | Description |
|-------------|-------------|
| `DOCKER_USERNAME` | Your Docker Hub username |
| `DOCKER_PASSWORD` | Docker Hub personal access token (PAT) |
| `RENDER_DEPLOY_HOOK` | Render deploy hook URL |

---

## 🚀 How It Works

1. `git push` to `main` branch
2. CI builds Docker image → pushes to Docker Hub
3. CD calls Render deploy hook → updates your live app

---

## 📎 Resources

- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [Render Deploy Hooks](https://render.com/docs/deploy-hooks)
- [Docker Hub](https://hub.docker.com/)
