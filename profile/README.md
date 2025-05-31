# SCOPE (System for Coordinated Operations & Police Engagement)
SCOPE is a Computer Aided Dispatch (CAD) and Mobile Data Terminal (MDT) system designed to streamline and coordinate law enforcement operations in real-time. It is built for use in roleplay environments like FiveM, but is scalable for real-world simulation and training scenarios. The system provides dispatchers and officers with a unified interface for managing calls, units, reports, and live data efficiently.

## Table of Contents
---
1. [Overview](#1-overview)  
2. [Getting Started](#2-getting-started)  
3. [Values and Priorities](#3-values-and-priorities)  
4. [Project Structure](#4-project-structure)  
5. [Technology Stack](#5-technology-stack)  
6. [Contributing](#6-contributing)
---

### 1. Goals and Objectives
Real-Time Coordination: Provide up-to-date information sharing between dispatchers and field units.

Efficient Workflow: Simplify and accelerate common police tasks such as traffic stops, incident reporting, and warrant checks.

Secure Access: Role-based access to maintain data integrity and operational security.

Auditability: Full logging of activities for administrative review.

### 2. User Roles
| Role           | Permissions                                                               |
| -------------- | ------------------------------------------------------------------------- |
| **Admin**      | Full system access, user management, audit logs                           |
| **Dispatcher** | Manage units, create/edit calls, assign priorities, broadcast BOLOs       |
| **Officer**    | Access MDT, search civilians/vehicles, submit reports, update unit status |
| **Supervisor** | Review reports, manage BOLOs, override decisions                          |
| **Civilian**   | (Optional module for record viewing or requests; e.g., FOIA simulation)   |

### 3. Values and priorititys
This project is designed with the following principles in mind:

✅ Open and Accessible
100% free and open-source stack.

No commercial or OS-dependent software required.

🛠 Cross-Platform Compatibility
Fully compatible with Windows, macOS, and Linux.

Uses only cross-platform libraries and tools.

🐳 Containerization with Docker
Includes a ready-to-use docker-compose.yml for PostgreSQL.

Encourages isolated, reproducible environments.

🗃 SQL-Based Storage (PostgreSQL)
Relies on PostgreSQL for robust, production-ready SQL storage.

Fully supported by Entity Framework Core using the Npgsql provider.

Easy to host, extend, and scale.

🧪 Testability and Maintainability
Repository pattern encourages clean separation of concerns.

Easily testable with mockable interfaces and minimal coupling.

♻️ Scalability
Structured to support future expansion:

API layer for endpoints.

Repository layer for data access.

Models layer for domain entities.

