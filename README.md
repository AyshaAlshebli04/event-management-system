# Event Management System

A robust, full-stack web application designed for comprehensive event scheduling and task tracking. This project was built utilizing **Java enterprise technologies** following a clean separation of concerns through architectural design patterns.

---

## Application Demonstration

Below is a complete visual walkthrough of the platform's core functional flows, including user onboarding, real-time data persistence, and event handling.

### Full System Walkthrough
[System Core Flows]
https://github.com/user-attachments/assets/acfd1aec-6354-4ba4-b6c3-dab97cf6bcc0


---

## Technical Architecture & Ecosystem

The backend implementation models an end-to-end relational ecosystem utilizing a modular object structure:

* **Architecture Pattern:** Model-View-Controller (MVC) to cleanly decouple data access from the presentation layers.
* **Backend Tier:** Java Servlets, JSP (JavaServer Pages), JDBC (Java Database Connectivity).
* **Database Layer:** Relational MySQL instance managing normalized table constraints.
* **Server Deployment:** GlassFish Server.

### Core File Structure Breakdown
```text
Event_Management_System/
├── src/java/com/eventapp/
│   ├── dao/          # Data Access Objects (EventDAO, UserDAO)
│   ├── model/        # Encapsulated Entities (User, Event)
│   ├── util/         # Database connection drivers (DBUtil)
│   └── web/          # HTTP Controllers (Login, Register, Logout Servlets)
└── web/              # Dynamic Presentation Layer (JSP views & custom CSS stylesheets)
