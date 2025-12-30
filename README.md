# Spring Boot Docker Setup

This repository contains the Docker configuration for running a Java Spring Boot application inside a Docker container.

## Prerequisites
- Docker Desktop installed and running
- Java 17 (only required if building locally without Docker)
- Maven (only required if building locally without Docker)

## Files Included
- Dockerfile: Multi-stage Dockerfile to build and run the Spring Boot application
- docker-compose.yml: Docker Compose file to build and run the container
- README.md: Setup and run instructions

## How to Build and Run Using Docker

1. Build and start the application using Docker Compose:
   docker-compose up --build

2. Once the container starts, access the application at:
   http://localhost:8080

## How to Stop the Application
- Press Ctrl + C in the terminal where Docker Compose is running
- Or run:
  docker-compose down

## Notes
- The Docker image uses a multi-stage build for a smaller image size
- The application behavior inside Docker matches the local Spring Boot run
- Port 8080 is exposed by default (update if your app uses a different port)
