# Fika Planner

**Plan Better Coffee Breaks Together**

Fika Planner is a web-based collaboration platform designed to simplify the organization of fika sessions among friends, university students, colleagues, and community groups.

Instead of coordinating through long conversations such as *"When are you free?"*, *"Where should we go?"*, and *"Who is coming?"*, Fika Planner provides a structured workflow for creating a fika, proposing cafés and times, voting on alternatives, managing attendance, and communicating with participants.

The project is developed as a production-oriented software engineering project, covering the complete development lifecycle from requirements analysis and UI/UX design through implementation, automated testing, CI/CD, deployment, and documentation.

---

## Project Goals

The main goal of Fika Planner is to demonstrate the development of a complete, maintainable, and deployable software system while solving a small but realistic coordination problem.

The project focuses on:

* Collaborative fika planning
* Secure authentication and authorization
* RESTful API design
* Relational database design
* Responsive and accessible user interface
* Automated testing
* Containerization
* CI/CD
* Cloud deployment
* Software architecture and technical documentation

---

## Core Features

### Account Management

* User registration
* Login and logout
* Profile management
* Authentication and authorization

### Fika Event Management

* Create a fika event
* Edit an event
* Cancel an event
* Discover upcoming events
* View past events

### Participation

* RSVP to events
* View participants
* Leave an event

### Collaborative Planning

* Suggest cafés
* Suggest suitable times
* Vote on cafés
* Vote on times
* Finalize the selected café and time

### Communication

* Event comments
* In-app notifications

### Administration

* User management
* Basic content moderation

---

## User Roles

The system initially supports three system-level roles:

| Role                | Description                                                         |
| ------------------- | ------------------------------------------------------------------- |
| **Guest**           | Can browse publicly available events and access registration/login. |
| **Registered User** | Can create and participate in fika events.                          |
| **Administrator**   | Can manage users and perform basic content moderation.              |

A registered user can act as an **event organizer** or **participant** depending on the event.

---

## System Architecture

The application follows a client-server architecture.

```text
┌─────────────────────────────┐
│     React + TypeScript      │
│          Frontend           │
└──────────────┬──────────────┘
               │
               │ REST / HTTPS
               ▼
┌─────────────────────────────┐
│       Spring Boot API       │
│                             │
│ Controllers                 │
│ Services                    │
│ Repositories                │
│ Security                    │
│ Validation                  │
└──────────────┬──────────────┘
               │
               │ SQL
               ▼
┌─────────────────────────────┐
│         PostgreSQL          │
│          Database           │
└─────────────────────────────┘
```

The backend is designed around separation of concerns and modular components, while the frontend provides a responsive web interface.

---

## Technology Stack

### Backend

* Java
* Spring Boot
* PostgreSQL
* REST API

### Frontend

* React
* TypeScript

### Testing

* JUnit
* Mockito
* Testcontainers
* Frontend testing framework

### DevOps

* Docker
* GitHub Actions
* Cloud deployment

### Documentation

* Markdown
* OpenAPI / Swagger
* Architecture Decision Records (ADRs)

---

## Project Documentation

The project is developed using a documentation-first approach. Important engineering decisions and specifications are maintained alongside the source code.

| Document                                              | Description                                                |
| ----------------------------------------------------- | ---------------------------------------------------------- |
| [Project Overview](docs/01-project-overview.md)       | Product vision, objectives, scope, users, and constraints  |
| [Requirements Specification](docs/02-requirements.md) | Functional and non-functional system requirements |

> Documentation will be updated throughout development as requirements and technical decisions evolve.

---

## Getting Started

### Prerequisites

The following tools are required to run the project locally:

* Java
* Node.js
* Docker
* Git

### Clone the repository

```bash
git clone <repository-url>
cd fika-planner
```

### Start the application

```bash
docker compose up
```

The exact setup instructions will be documented here as the implementation is completed.

---

## Testing

Testing is treated as an integral part of the development process rather than a final project phase.

The project will include:

* Unit tests
* Integration tests
* Database integration tests using Testcontainers
* Frontend tests
* API-level testing

The CI pipeline will automatically execute the relevant tests when changes are pushed to the repository.

---

## CI/CD

The project uses GitHub Actions to automate the development workflow.

The intended pipeline is:

```text
Code Push
    │
    ▼
Build
    │
    ▼
Unit Tests
    │
    ▼
Integration Tests
    │
    ▼
Frontend Tests
    │
    ▼
Docker Build
    │
    ▼
Deployment
```

---

## Live Application

**Application:** Coming soon

**API Documentation:** Coming soon

**Deployment:** Coming soon

---

## MVP Scope

The initial release focuses on the core functionality required to plan and organize a fika.

The MVP prioritizes:

* Core user workflows
* Security
* Usability
* Data integrity
* Automated testing
* Deployment
* Documentation

The following are intentionally excluded from the initial MVP:

* Real-time collaboration
* External calendar integrations
* Sophisticated recommendation systems
* Mobile applications

These may be considered as future improvements.

---

## Future Possibilities

Potential future enhancements include:

* Google Calendar and Outlook integration
* Email notifications
* Real-time voting using WebSockets
* Interactive café maps
* Recurring fika events
* External café information integration
* Personalized café recommendations
* Mobile application
* Workplace/team integrations

---

## Project Status

**Status:** In Development

The project is being developed as an individual software engineering project with an emphasis on completing a small, production-oriented system rather than building a large number of features.

> **Quality over quantity.**

The objective is to demonstrate the complete journey from an initial product idea through requirements analysis, design, implementation, testing, deployment, and documentation.

---

## License

This project is developed as a personal software engineering portfolio project.

License information will be added before the first public release.

