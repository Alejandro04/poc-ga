# GitHub Actions PoC for Docker Build and Push

This repository is a **Proof of Concept (PoC)** demonstrating how to leverage **GitHub Actions** for building and pushing Docker images to **Docker Hub** automatically. The goal is to explore and test the capabilities of GitHub Actions in continuous integration (CI) and continuous deployment (CD) workflows.

## Overview

In this project, I'm experimenting with setting up a GitHub Actions workflow that:

- Builds a Docker image from a `Dockerfile` every time changes are pushed to the `master` branch.
- Pushes the resulting Docker image to my Docker Hub repository.
  
The workflow is triggered automatically on every `push` or `pull request` to the `master` branch, making the process seamless and fully automated.

## Key Technologies

- **GitHub Actions**: Automating the CI/CD process.
- **Docker**: Containerizing the application using a `Dockerfile`.
- **Docker Hub**: Pushing built images to Docker Hub for easy access and deployment.

## How It Works

1. **Build**: GitHub Actions automatically builds the Docker image using the `Dockerfile` provided in the repository.
2. **Push**: Once the image is built, it is pushed to my Docker Hub account using secure credentials stored in GitHub Secrets.
3. **Triggering**: The workflow is triggered by:
   - A push to the `master` branch.
   - A pull request to the `master` branch.

