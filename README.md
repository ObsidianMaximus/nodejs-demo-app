# Node.js Demo App CI/CD Pipeline

A demo Node.js app with automated CI/CD using GitHub Actions and Docker.

---

## 🚀 Features

- Runs tests on every push to `master` (or manually).
- Builds and publishes a Docker image to GitHub Container Registry (GHCR)
- Easy one-line deployment

---

## 🛠️ CI/CD Workflow

- **Test:** Installs dependencies and tests the application.
- **Build & Deploy:** Builds the Docker image and pushes it to the GHCR repository.

---

## 🐳 Usage

### Pull and Run from GHCR
```bash
docker pull ghcr.io/obsidianmaximus/nodejs-demo-app:latest
docker run -p 80:5006 ghcr.io/obsidianmaximus/nodejs-demo-app:latest
```

### Build and Run Locally
```bash
docker build -t nodejs-demo-app .
docker run -p 80:5006 nodejs-demo-app
```

---

## 🔒 Setup

- Add a `GHCR_TOKEN` secret in your repo for publishing to GHCR.

---

## 📄 Files

- `.github/workflows/main.yml` — CI/CD workflow
- `Dockerfile` — Container build instructions

---

**Good luck! :)**