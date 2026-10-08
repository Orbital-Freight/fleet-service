# Fleet Service

Microservice responsible for managing the fleet in the Orbital Freight ecosystem.

## Tech Stack

- **Java**: 25
- **Framework**: Spring Boot 4.1.x
- **Database**: PostgreSQL 18 (H2 for unit tests)
- **Containerization**: Docker & Docker Compose
- **Development Environment**: VS Code Dev Containers

## Getting Started

### Prerequisites

- Docker & Docker Compose (or VS Code with Dev Containers extension)
- Java 25 & Maven 3.9+ (if running directly on the host)

### Running with Docker Compose

To start the fleet service along with the PostgreSQL database:

```bash
docker compose up --build
```

The service will be accessible at `http://localhost:8080`.

### Development via Dev Container

1. Open this repository in Visual Studio Code.
2. When prompted, select **Reopen in Container** (or run `Dev Containers: Reopen in Container` from the command palette).
3. The container comes pre-configured with Java 25, Docker-outside-of-Docker, and essential extensions.

### Running Tests

Within the Dev Container or host with Java 25:

```bash
./mvnw clean test
```