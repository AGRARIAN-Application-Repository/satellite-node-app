# satellite-node-app

Agrarian satellite-node-app Application

## Description

This is a simple FastAPI application for the Agrarian ecosystem.

## Local Development

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
python src/app.py
```

## Docker

```bash
# Build the image
docker build -t satellite-node-app .

# Run the container
docker run -p 80:80 satellite-node-app
```

## CI/CD

This repository uses a simple CI/CD pipeline that:
- Tests application compilation
- Checks for hardcoded secrets
- Builds Docker image
- Pushes to GitHub Container Registry
- Tests the Docker image

## Endpoints

- `GET /` - Main endpoint
- `GET /health` - Health check
