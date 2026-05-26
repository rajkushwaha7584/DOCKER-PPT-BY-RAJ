# Docker Presentation by Raj

This repository contains a complete Docker presentation created for learning, interview preparation, and DevOps understanding.

The goal of this project is to explain Docker in a simple and practical way, including Docker basics, containers, images, Dockerfile, Docker Compose, networking, volumes, registry, monitoring, and commonly used Docker commands.

---

## About Docker

Docker is a containerization platform used to package an application with all its required dependencies, libraries, and runtime.

It helps developers run applications in the same environment everywhere.

Docker solves the common problem:

> "It works on my machine, but not on the server."

---

## Topics Covered

- What is Docker?
- Docker vs Virtual Machine
- Docker Architecture
- Docker Engine
- Docker Image
- Docker Container
- Dockerfile
- ENTRYPOINT vs CMD
- Multi-stage Dockerfile
- Docker Compose
- Docker Networks
- Docker Volumes
- Docker Registry
- Docker Monitoring and Logs
- Docker Scout
- Important Docker Commands

---

## Docker vs Virtual Machine

| Feature | Docker Container | Virtual Machine |
|---|---|---|
| OS Usage | Shares the host OS kernel | Runs a complete separate OS |
| Size | Lightweight, usually MBs | Heavy, usually GBs |
| Startup Time | Starts in seconds | Takes minutes to start |
| Performance | Faster and efficient | Slower compared to containers |
| Resource Usage | Uses less CPU and RAM | Uses more CPU and RAM |
| Isolation | Process-level isolation | Full machine-level isolation |
| Use Case | App deployment, microservices, CI/CD | Running different OS and full server setup |

---

## Docker Architecture

| Component | Simple Explanation |
|---|---|
| Docker Client | Used to run Docker commands like `docker build`, `docker run`, and `docker ps`. |
| Docker Daemon | Runs in the background and manages images, containers, networks, and volumes. |
| Docker Image | A read-only template that contains app code, dependencies, and runtime. |
| Docker Container | A running instance of a Docker image. |
| Docker Registry | A place where Docker images are stored and managed. |
| Docker Hub | Public Docker registry where ready-made images are available. |

---

## Docker Engine

Docker Engine is the core software of Docker.

It is responsible for building images, running containers, and managing Docker resources like networks and volumes.

Main parts of Docker Engine:

| Part | Explanation |
|---|---|
| Docker CLI | Command-line tool used by the user |
| Docker Daemon | Background service that manages Docker objects |
| REST API | Helps CLI communicate with Docker Daemon |

---

## Docker Image

A Docker Image is a read-only package that contains everything needed to run an application.

It includes:

- Application code
- Libraries
- Dependencies
- Runtime
- Configuration

Example:

```bash
docker pull nginx
