📘 StudyBlog — Personal Study Journey Blog

StudyBlog is a full-stack project created to publicly document my study journey in technology (Java, Spring, Backend, etc.). It works as a personal technical blog, organized by topics and supported by a learning roadmap.

The project was designed as a realistic MVP, focused on backend best practices, security, and clean architecture, simulating a system that could be used in a production environment.

🎯 Project Goal

Document and share my technical learning journey

Organize content by topics (e.g., Java, Spring, SQL)

Display a visual learning roadmap of completed and upcoming topics

Allow post creation only by the administrator

Serve as a portfolio project for Java backend positions

🧩 Features
🔓 Public

View list of published posts

Read full posts by slug

Browse study topics

View learning roadmap by topic

🔐 Admin (author only)

Login with JWT authentication

Create draft posts

Publish / unpublish posts

Create and manage topics

Create and update roadmap items

🛠️ Tech Stack
Backend

Java 17

Spring Boot 3

Spring Web

Spring Data JPA (Hibernate)

Spring Security + JWT

Flyway (database versioning)

PostgreSQL

Maven

Frontend (in progress)

Angular (standalone components)

REST API consumption

🗂️ Architecture

The backend follows a layered architecture with a clear separation of concerns:

Controllers: HTTP layer

Services: business rules

Repositories: data access

DTOs: input/output contracts

Security: JWT-based authentication and authorization

🔐 Security

JWT-based authentication

Clearly defined public and protected routes

/api/public/** → open access

/api/admin/** → requires JWT token

Stateless session (REST standard)

🗄️ Database

PostgreSQL

Versioned with Flyway

Automatic schema creation on application startup

Full control of the data model via SQL migrations

DEPLOY → coming soon 🚀
