AI Intelligent Note Pro - Ultra Dashboard
AI Intelligent Note Pro is a cutting-edge, microservice-based ecosystem designed to transform traditional note-taking into a cognitive behavioral analysis tool. The platform utilizes a deterministic AI engine to evaluate user thought patterns and provide real-time cognitive insights.

<img width="945" height="461" alt="image" src="https://github.com/user-attachments/assets/6fb5a57c-11a5-453d-8e13-53c1b7b42e9b" />


 Project Overview
This project implements a high-performance microservice stack, orchestrated with Docker, secured with JWT, and automated via a robust CI/CD pipeline. It features a "Cognitive Intelligence Dashboard" that analyzes user data to determine brain dominance and memory metrics.

 Key Features
Cognitive AI Engine: Analyzes user inputs to calculate Retention, Detail, and Speed scores.

Brain Dominance Analysis: Visualizes "Left-Brained" vs "Right-Brained" tendencies using dynamic SVG filters.

Microservice Architecture: Decoupled services for Auth, Note Management, and Notifications.

Asynchronous Communication: Inter-service communication via HTTPX for high-efficiency email delivery.

Pro Dashboard UI: A modern, glassmorphic interface built with Chart.js and Plus Jakarta Sans.

 Technical Architecture and Infrastructure
 <img width="945" height="516" alt="image" src="https://github.com/user-attachments/assets/50e5b269-cfe9-4016-a608-cdd8bdbea458" />

The system follows a Clean Architecture pattern, ensuring separation of concerns across multiple layers:

API Layer (FastAPI): Handles request routing, Pydantic validation, and authentication.

Core Logic (Service Layer): Executes business rules and the AI cognitive scoring algorithm.

Database Layer (SQLAlchemy): Manages persistent storage with PostgreSQL/SQLite.

Gateway (Nginx): Acts as a reverse proxy, orchestrating traffic between services.

<img width="914" height="284" alt="image" src="https://github.com/user-attachments/assets/e9126675-78fa-429d-94fa-6d0d27f05c80" />
<img width="945" height="453" alt="image" src="https://github.com/user-attachments/assets/f9e17e9e-c0be-4492-a810-22c4bb7ce70d" />


AI PART SYSTEMS BASIC DEFINATION 
<img width="945" height="365" alt="image" src="https://github.com/user-attachments/assets/a6a68446-9b85-43f4-9cfb-8fac323f63ee" />
SOURCES 
Mueller, P. A., & Oppenheimer, D. M. (2014). The pen is mightier than the keyboard. Psychological Science, 25(6), 1159-1168.
 Tulving, E., et al. (1994). Hemispheric encoding/retrieval asymmetry in episodic memory. PNAS, 91(6), 2016-2020.
Rathod et al. (2016)
“Novel insights into the effect of vitamin B12 and omega-3 fatty acids on brain function”




1. Complete CI/CD Pipeline
We implemented a professional pipeline using GitHub Actions. Every "push" to the main branch triggers:

Environment Setup: Virtual environment and dependency installation.

Linting & Formatting: Code quality checks.

Automated Testing: Execution of the test suite.

Container Build: Verification of Docker images.

2. Automated Testing
The system includes automated unit tests that validate the AI Logic Engine and API Endpoints. This ensures that cognitive score calculations remain accurate through every update.

3. Container Orchestration
The entire stack is containerized using Docker. Deployment is managed via Docker Compose, ensuring a "cloud-like" environment where services are isolated, health-checked, and network-linked.

 Getting Started
Prerequisites
Docker & Docker Compose

Bash
docker-compose up --build
Access the Dashboard:
Open http://localhost/static/index.html in your browser.
<img width="1893" height="912" alt="image" src="https://github.com/user-attachments/assets/cfaf50b1-cdc2-4c1e-b8d1-1dab4a767240" />


docker-compose up --build
Access the Dashboard:
Open http://localhost/static/index.html in your browser.
