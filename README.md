# 💬 Chat Messenger

A full-stack **chat messenger** application designed for **real-time communication**, built with **Java**, **Spring Boot**, and **WebSocket protocols**, offering secure messaging with a clean RESTful architecture. This is an ongoing project with an already developed backend and a frontend under active design.

---

## 🧱 Tech Stack

| Layer         | Technologies Used                                                                                                                                   |
|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Backend**   | Java 17, Spring Boot 3.x, Spring WebSocket, Spring Security, Spring Data JPA, JWT, SpringDoc OpenAPI/Swagger, PostgreSQL/MySQL                     |
| **Messaging** | WebSocket (STOMP), SimpleBroker (✅), RabbitMQ (🚧 planned upgrade)                                                                                   |
| **Real-Time** | WebSocket Protocols, STOMP                                                                                                                          |
| **Future Additions** | Kafka (for logging, scalability, and event-driven design), Redis (optional for session/cache optimization)                                               |
| **Frontend**  | (🚧 In progress) Vaadin-based UI + Figma/UX tools for professional UI/UX design                                                                      |
| **DevOps**    | Maven, GitHub Codespaces Support , Docker                                                                                                                |

---

## ✨ Features

### ✅ Features
- **Real-Time Messaging** via Spring WebSocket
- **JWT Authentication** & Role-Based Access
- **RESTful APIs** for User, Session, and Message Management
- **Message Sessions**: Communication is session-based with unique session IDs
- **Message Storage**: Messages are saved as **JSON objects** in the database
- **Structured API Responses** with detailed status and messages
- **Integrated Swagger Docs** with live examples
- **Custom Exception Handling** for better error visibility

### 🚧 Future Features
- **RabbitMQ Integration** for advanced messaging broker capabilities
- **Kafka-Based Logging** for auditing & analytics
- **Encrypted Message Storage** using AES/GCM encryption
- **Frontend Client** with modern UI/UX (Figma prototyping + Vaadin/React)
- **Advanced Authorization Rules** with granular permission checks
- **Multi-language Support** (English-Persian planned)

---

## Architecture

```
+-------------+      WebSocket/STOMP     +---------------+
|   Frontend  | <----------------------> | Spring Boot    |
|   (Vaadin)  |                          | + WebSocket    |
+-------------+                          +---------------+
        |                                       |
        | REST API (JWT)                        |
        v                                       v
+---------------+                        +---------------+
|   User Auth   |                        | Message Broker |
|   Service     |                        | (SimpleBroker /|
+---------------+                        | RabbitMQ)      |
        |                                       |
        v                                       v
+----------------------------------------------+
|             PostgreSQL / MySQL               |
|       Users | Sessions | Messages (JSON)     |
+----------------------------------------------+
```

## 🧑‍💻 Contributors

A collaborative effort by an enthusiastic team:

- **Morteza Mahdi Zadeh** (Lead Developer)
- **Soheil Nouhi**
- **Mohamad Reza Asgari**
- **Ali Sedighi**
- **Ehsan Shahsavari**
- **Daniel Khalaji**

---

## 🚀 Getting Started

### 🔧 Prerequisites
- Java 17+
- Maven 3.x
- PostgreSQL or MySQL

### 📦 Installation
