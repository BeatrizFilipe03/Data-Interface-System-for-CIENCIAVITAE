# Data Interface System for CIÊNCIAVITAE

This project aims to facilitate the management and interoperability of academic CVs, with a focus on integration with the [CIÊNCIAVITAE](https://cienciavitae.pt/) platform. It provides a modern web application composed of a Kotlin/Spring Boot backend and a React/TypeScript frontend, allowing users to import, edit, and export CV data in a structured and efficient way.

📄 **[Full project report (in Portuguese)](docs/rfG28.pdf)** - architecture, data model, technologies, implementation and tests.

## Key Features

- Import academic CVs from external platforms such as Lattes (Brazil) via XML.
- Visualize structured CV data in an intuitive web interface.
- Export CVs to the CIÊNCIAVITAE platform using its official API.
- Store user data in a PostgreSQL relational database with structured entity mapping.
- Built with a modular and extensible architecture, enabling future integration with other platforms.

This system is designed to support researchers, academic institutions, and organizations in avoiding data duplication and ensuring high data quality.

## 📦 Project Structure
```
.
├── backend/        # Kotlin Spring Boot application
├── frontend/       # React + TypeScript web client
├── docker-compose.yml
```

---

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Running with Docker Compose

From the root of the project, run:

```bash
docker compose up --build
```

This will:
- Start the backend (on port 8081)
- Start the frontend (on port 3000)
- Start the PostgreSQL database (on port 5432)

### Accessing the Application

Frontend: http://localhost:3000

Backend API (Swagger UI): http://localhost:8081/swagger-ui.html
