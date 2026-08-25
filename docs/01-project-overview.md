
# Fika Planner

**Plan Better Coffee Breaks Together**


## Table of Contents

1. [Project Overview](#1-project-overview)
2. [Problem Statement](#2-problem-statement)
3. [Proposed Solution](#3-proposed-solution)
4. [Project Objectives](#4-project-objectives)
5. [Target Users](#5-target-users)
6. [User Roles](#6-user-roles)
7. [Core User Journey](#7-core-user-journey)
8. [Core Features](#8-core-features)
9. [Project Scope](#9-project-scope)
10. [Technical Goals](#10-technical-goals)
11. [Success Criteria](#11-success-criteria)
12. [Project Constraints](#12-project-constraints)
13. [Future Possibilities](#13-future-possibilities)

---

## 1 Project Overview

Fika Planner is a web-based collaboration platform designed to simplify the organization of fika sessions among friends, university students, colleagues, and community groups.

The application provides a centralized place where users can create fika events, invite or share events with others, propose suitable cafes and times, vote on alternatives, manage attendance, and communicate with participants. The goal is to reduce the back-and-forth communication commonly involved in organizing informal social gatherings.

The project is designed as a production-oriented software engineering project, covering the complete development lifecycle from requirements analysis and UX/UI design through implementation, automated testing, CI/CD, deployment, and documentation.

## 2 Problem Statement

Fika is an important part of Swedish social and workplace culture, but organizing a fika with a group can still involve unnecessary coordination.

A typical conversation might involve:

> "When are you free?"
> "How about Friday?"
> "What time?"
> "15:00 works for me."
> "Where should we go?"
> "I don't mind."
> "How about Cafe X?"
> "Too far for me."
> "Okay, Cafe Y?"

When several people are involved, these conversations can become difficult to follow and decisions can be unclear.

Existing general-purpose communication and event platforms can be used for this purpose, but they are not specifically designed around the lightweight decision-making process involved in organizing a fika.

Fika Planner addresses this problem by providing a focused workflow for planning, deciding, and participating in fika events.

## 3 Proposed Solution

Fika Planner allows a user to create a fika event and define possible dates, times, and locations.

Participants can then:

- View the event
- Indicate whether they are attending
- Suggest cafes
- Vote on proposed cafes
- Vote on proposed times
- Discuss the event
- Receive relevant notifications

Once sufficient responses have been collected, the organizer can finalize the fika details.

The application therefore transforms an informal group discussion into a structured but lightweight planning process.

## 4 Project Objectives

The main objective is to develop a fully functional, maintainable, and deployable web application that demonstrates professional software engineering practices.

Specific objectives are to:

1. Provide a simple way to organize fika events.
2. Reduce communication overhead when selecting a time and location.
3. Allow participants to collaboratively make decisions.
4. Provide appropriate access control for different types of users.
5. Develop a responsive and accessible user interface.
6. Implement a secure REST API.
7. Apply automated unit and integration testing.
8. Establish a reproducible development and deployment process.
9. Deploy the application to a publicly accessible environment.
10. Document the system and its technical decisions.

## 5 Target Users

The initial target audience consists of people who regularly organize informal group gatherings.

- **University Students** — Students can organize fika sessions with classmates, study groups, or student organizations.
- **Employees and Teams** — Teams can use Fika Planner to organize informal workplace fika without lengthy conversations in workplace communication channels.
- **Friends and Social Groups** — Friends can use the application to decide when and where to meet.
- **Community Groups** — Small clubs, associations, and other informal groups can use the platform for recurring social gatherings.

## 6 User Roles

The system will initially support three access levels.

1. **Guest**
   - An unauthenticated visitor who can browse publicly available fika events and view basic event information.
   - Guests cannot participate in events or create events until they register and authenticate.
2. **Registered User**
   - An authenticated user who can participate in fika events and create their own events.
   - A registered user can act as both a participant and an organizer, depending on the event.
3. **Administrator**
   - A privileged user responsible for basic platform administration and moderation.
   - Administrators can manage users and moderate inappropriate content.

## 7 Core User Journey

The core journey represents the core business flow of the application. The primary user journey is as follows.

```
Discover Fika Planner
        ↓
Browse public events
        ↓
Register / Login
        ↓
Create or join a fika
        ↓
Propose cafes and times
        ↓
Vote
        ↓
RSVP
        ↓
Organizer finalizes the plan
        ↓
Attend the fika
        ↓
Leave feedback
```

## 8 Core Features

The initial version of Fika Planner will include the following core features.

1. **Account Management**
   - Registration
   - Login/logout
   - Profile management
   - Authentication and authorization
2. **Event Management**
   - Create fika
   - Edit fika
   - Cancel fika
   - View upcoming and past events
3. **Participation**
   - RSVP
   - View participants
   - Leave an event
4. **Collaborative Planning**
   - Suggest cafes
   - Suggest times
   - Vote on cafes
   - Vote on times
   - Finalize the selected options
5. **Communication**
   - Event comments
   - In-app notifications
6. **Administration**
   - User management
   - Basic content moderation

## 9 Project Scope

The project will focus on developing a Minimum Viable Product (MVP) that demonstrates the core functionality of the platform while remaining achievable within the planned development period.

The MVP will prioritize:

- Core user workflows
- Security
- Usability
- Data integrity
- Automated testing
- Deployment
- Documentation

Advanced functionality such as real-time collaboration, external calendar integrations, sophisticated recommendation systems, and mobile applications will not be part of the initial MVP.

These features may be considered as future improvements.

## 10 Technical Goals

Although Fika Planner is primarily a product concept, the project is also intended to demonstrate professional software engineering practices.

The system will therefore emphasize:

- Modular backend architecture
- RESTful API design
- Secure authentication and authorization
- Relational database design
- Separation of concerns
- Automated testing
- Containerization
- CI/CD
- Code quality
- Observability and error handling
- API documentation
- Maintainable frontend architecture

### Planned Technology Stack

**Backend**
- Java
- Spring Boot
- PostgreSQL

**Frontend**
- React
- TypeScript

**Testing**
- JUnit
- Mockito
- Testcontainers
- Frontend testing framework

**DevOps**
- Docker
- GitHub Actions
- Cloud deployment

## 11 Success Criteria

The project will be considered successful when:

- A new user can register and authenticate.
- An authenticated user can create a fika event.
- Other users can discover and join the event.
- Participants can propose and vote on cafés and times.
- The organizer can finalize the fika.
- Unauthorized users cannot perform protected operations.
- Core backend functionality is covered by automated tests.
- The application is deployed and accessible online.
- The project can be started locally using documented instructions.
- The architecture, requirements, API, testing strategy, and deployment process are documented.

## 12 Project Constraints

The project is intended to be developed as an individual software engineering project within approximately 10 days.

Therefore, the project will prioritize **quality over quantity**.

The goal is not to build a large social platform, but to produce a small, complete, production-oriented system demonstrating the ability to move from an initial idea through design, implementation, testing, and deployment.

## 13 Future Possibilities

Potential future versions could include:

- Google/Outlook calendar integration
- Email notifications
- Real-time voting using WebSockets
- Interactive café maps
- Recurring fika events
- Public café information integration
- Personalized café recommendations
- Accessibility improvements
- Mobile application
- Team/workplace integrations

These features are deliberately excluded from the initial scope so that the MVP can be completed and properly tested.
