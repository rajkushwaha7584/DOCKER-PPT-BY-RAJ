# Docker Complete Presentation by Raj

This repository contains a complete Docker presentation prepared for learning, revision, and interview preparation.  
It explains Docker concepts in simple English with examples, commands, and real-world DevOps use cases.

---

## About This Presentation

Docker is one of the most important tools in DevOps.  
It helps developers and DevOps engineers package applications with all required dependencies and run them in isolated containers.

This presentation covers Docker from basic to advanced level in a simple and practical way.

---

## Topics Covered

- What is Docker?
- Why Docker is used
- Docker vs Virtual Machine
- Docker Architecture
- Docker Engine
- Docker Image
- Docker Container
- Dockerfile
- ENTRYPOINT vs CMD
- Docker build and run commands
- Multi-stage Dockerfile
- Docker Compose
- Docker Network
- Docker Volume
- Docker Registry
- Docker Hub
- Docker Monitoring and Logs
- Docker Scout
- Useful Docker commands
- Docker installation on Linux
- Real-world Java application example

---

## Docker Definition

Docker is a platform used to build, package, and run applications inside containers.

A container includes the application code, dependencies, libraries, and runtime required to run the application.

---

## Why Docker is Used

Docker is used to solve the common problem:

> "It works on my machine, but not on the server."

With Docker, the application runs in the same environment everywhere:
developer laptop, testing server, production server, or cloud.

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
| Portability | Easy to move across systems | Less portable because of full OS |
| Best Use Case | App deployment, microservices, CI/CD | Running different OS and full server setup |

---

## Docker Architecture

Docker architecture mainly contains:

| Component | Simple Explanation |
|---|---|
| Docker Client | Tool used to run Docker commands like `docker build`, `docker run`, and `docker ps`. |
| Docker Daemon | Background service that builds images, runs containers, and manages Docker resources. |
| Docker Image | Read-only template that contains application code, dependencies, and runtime. |
| Docker Container | Running version of a Docker image. |
| Docker Registry | Storage place where Docker images are stored and managed. |
| Docker Hub | Public Docker registry where ready-made images are available. |

---

## Docker Engine

Docker Engine is the core software of Docker.  
It builds images, runs containers, and manages Docker resources like networks and volumes.

Main parts of Docker Engine:

| Part | Explanation |
|---|---|
| Docker CLI | Command line tool used by users |
| Docker Daemon | Background service that manages Docker |
| REST API | Helps CLI communicate with Docker Daemon |

---

## Docker Image

A Docker image is a read-only template that contains application code, libraries, dependencies, and runtime.

Example:

```bash
docker pull nginx
