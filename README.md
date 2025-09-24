# 🚀 My First CI/CD Web App with Jenkins, GitHub & Docker

This project is a super simple web app to test CI/CD pipeline.

## How it works
1. Code lives here on GitHub.
2. Jenkins pulls code when I push (via webhook).
3. Jenkins builds a Docker image using `Dockerfile`.
4. Jenkins runs a container on port **8081** with Nginx serving `index.html`.

## Run locally (optional)
```bash
docker build -t nginx-image1 .
docker run -d -p 8081:80 --name=container1 nginx-image1
