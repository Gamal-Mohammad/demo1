# Demo1 – Spring Boot REST API

![Java](https://img.shields.io/badge/Java-007396?logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/Spring-6DB33F?logo=spring&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

> Minimal Spring Boot REST service for managing `Person` records, packaged with Docker.

## Overview

A small **Spring Boot 2.3** application exposing a `Person` REST API (`/persons/all`) on port **8090**, with a controller / service / model layout, a Maven wrapper and a Dockerfile.

## Tech Stack

- **Java**
- **Spring**
- **Maven**
- **Docker**

## API

| Method | Endpoint | Description |
|---|---|---|
| GET | `/persons/all` | List all persons |

## Repository Structure

```text
.gitignore
Dockerfile
mvnw
mvnw.cmd
pom.xml
README.md
src/main/java/ …
src/main/resources/ …
src/test/java/ …
```

## Getting Started

```bash
./mvnw clean package
docker build -t demo1 .
docker run -d -p 8090:8090 demo1
curl http://localhost:8090/persons/all
```

## Author

**Gamal Mohammad**

[![GitHub](https://img.shields.io/badge/GitHub-Gamal--Mohammad-181717?logo=github)](https://github.com/Gamal-Mohammad)
