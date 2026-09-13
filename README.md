# Quantum Leap

Quantum Leap project repository.

## Docker Setup

### Local Build & Run
To build and run the Docker container locally:
```bash
docker build -t quantum-leap .
docker run -p 8000:8000 quantum-leap
```

### Automated Builds with Docker Hub
This repository is configured with a GitHub Actions workflow (`.github/workflows/docker-build.yml`) to automatically build and push Docker images to Docker Hub on push to `main`.

To enable automated push:
1. Go to your repository settings on GitHub: **Settings > Secrets and variables > Actions**.
2. Add the following repository secrets:
   - `DOCKERHUB_USERNAME`: Your Docker Hub username.
   - `DOCKERHUB_TOKEN`: A Personal Access Token generated from Docker Hub (**Account Settings > Personal Access Tokens**).
