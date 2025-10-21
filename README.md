# Auto Deploy Portfolio Website

A simple portfolio website that automatically deploys using GitHub Actions and Docker.

## How it works
- On every push to main branch, GitHub Actions builds and pushes a Docker image to Docker Hub.
- The portfolio runs on Nginx inside a Docker container.

## Run locally
```
docker build -t manoj-portfolio .
docker run -d -p 8080:80 manoj-portfolio
```
