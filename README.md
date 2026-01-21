# NAME: KARTHIK S, REG NO: 23BCE1260
# 23BCE1260-SOFTWARE-PROJECT-ARCHITECT_LIVE 
# ArchitectLive – Collaborative Infrastructure-as-Code Platform

## 1. Project Overview
**ArchitectLive** is a web-based "No-Code" development environment that bridges the gap between high-level system design and low-level implementation. It allows software engineers to design distributed systems visually on a drag-and-drop canvas and—with a single click—transform that diagram into a fully functional, production-ready Infrastructure-as-Code (IaC) bundle.

## 2. Problem It Solves
* **The "Blank Screen" Paralysis:** Setting up microservices (e.g., linking React to Node/Postgres) requires writing complex configuration files (Docker Compose, K8s manifests) before writing any business logic.
* **Configuration Drift:** Teams often suffer from "it works on my machine" issues due to inconsistent local environment setups.
* **Documentation Disconnect:** System diagrams on whiteboards or tools like Lucidchart are static images that quickly become outdated and disconnected from the actual codebase.

## 3. Target Users (Personas)
* **Junior Developers / Students:** Who find DevOps and network configuration intimidating and prone to syntax errors.
* **System Architects:** Who need to rapidly prototype architectures and enforce design standards across teams.
* **Hackathon Teams:** Who need to spin up a full-stack boilerplate in minutes, not hours.

## 4. Vision Statement
To empower developers to build complex cloud infrastructure as easily as drawing a flowchart, eliminating the barrier between architectural thought and executable code.

## 5. Key Features / Goals
* **Visual Canvas:** Interactive drag-and-drop interface for service nodes (React, Node.js, Python, Databases).
* **Intelligent Linking:** Automatic protocol detection (HTTP/TCP) and dependency injection when connecting nodes.
* **Logic Engine:** Real-time validation to prevent invalid architectures (e.g., cyclic dependencies).
* **One-Click Compiler:** Generates a downloadable ZIP artifact containing `docker-compose.yml`, `Dockerfile`, `.env`, and boilerplate code.
* **GitHub Integration:** Direct export of generated code to a new GitHub repository.

## 6. Success Metrics
* **Speed:** Users should be able to generate a runnable "Hello World" full-stack environment in under 5 minutes.
* **Accuracy:** Generated code must be syntax-error-free and deployable via `docker-compose up` 100% of the time.
* **Adoption:** 80% of beta users successfully export a project without consulting the manual.

## 7. Assumptions & Constraints
* **Constraint:** The "Live Test" feature requires Docker-in-Docker privileges on the host server.
* **Assumption:** Users have Docker Desktop installed locally to run the downloaded artifacts.
* **Constraint:** Initial support is limited to the MERN stack and Python/PostgreSQL services.

## Branching Strategy

We follow the GitHub Flow branching strategy:

- The `main` branch contains production-ready code.
- All new features are developed in feature branches.
- Feature branches follow the format: `feature/feature-name`
  Examples:
  - `feature/canvas-drag-drop`
  - `feature/docker-setup`
- Feature branches are merged into `main` using Pull Requests after review.

> Canvas drag-and-drop feature under development.
>
> ## Local Development Tools

The following tools were used to develop and run ArchitectLive locally:

- **Docker Desktop** – For containerizing and running the frontend and backend services
- **Docker Compose** – To orchestrate multi-container application setup
- **Git & GitHub** – For version control, branching strategy, and collaboration
- **Node.js** – Backend runtime environment
- **Express.js** – Lightweight web framework for backend services
- **VS Code** – Code editor for development
- **Windows OS** – Local development environment

