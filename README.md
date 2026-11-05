# 🚀 TaskFlow – Smart Task Management & Productivity Tracking System

<p align="center">
  <strong>Plan Smart. Work Better. Achieve More.</strong>
</p>

<p align="center">
  A web-based task management application built using Node.js, Express.js, MongoDB and Docker.
</p>

---

## 👨‍💻 Project Information

| Detail | Information |
|---|---|
| Project Title | TaskFlow – Smart Task Management & Productivity Tracking System |
| Subject | Web Programming |
| Assignment | Assignment 2 |
| Frontend | HTML, CSS, JavaScript |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| ODM | Mongoose |
| Containerization | Docker, Docker Compose |

### Project Team

| Name | Roll Number |
|---|---|
| **G. Sriram Charan** | **24071A6691** |
| **Mahender Reddy** | **24071A6684** |

---

## 🎥 Project Demonstration Video

Watch our complete project demonstration covering the project objectives, features, technologies used, backend implementation, database integration, Docker configuration, and live application demo.

<p align="center">
  <a href="https://drive.google.com/file/d/1q7xqCZMVSNod560dq2GQKg9I_MEExsFQ/view?usp=sharing">
    <strong>▶️ WATCH TASKFLOW PROJECT DEMONSTRATION</strong>
  </a>
</p>

**Video Link:**  
https://drive.google.com/file/d/1q7xqCZMVSNod560dq2GQKg9I_MEExsFQ/view?usp=sharing

---

## 📌 1. Project Overview

TaskFlow is a web-based task management and productivity tracking application designed to help users organize their daily activities, manage priorities, monitor task progress, and improve productivity.

The application provides an interactive dashboard where users can create, update, delete, categorize, and track their tasks.

It integrates a Node.js and Express.js backend with a MongoDB database for persistent data storage. Docker is used to containerize the application and database, making the project easier to configure and run.

### 🎯 Project Objectives

- Develop an interactive task management platform.
- Simplify task creation and organization.
- Manage tasks based on priority and status.
- Track time spent on individual tasks.
- Visualize productivity through dashboard analytics.
- Implement backend CRUD operations.
- Integrate MongoDB for persistent storage.
- Use Docker for containerization and application management.

---

## ✨ 2. Key Features

### 📊 Interactive Dashboard
- Overview of total, pending, and completed tasks.
- Productivity statistics.
- Centralized task management interface.

### 📝 Task Management
- Create new tasks.
- Edit existing task details.
- Delete unnecessary tasks.
- Add descriptions, categories, priorities, and due dates.

### 📋 Kanban Board
- Organize tasks into three stages:
  - To Do
  - In Progress
  - Done
- Move tasks between stages using drag and drop.

### ⏱️ Time Tracking
- Start and stop task timers.
- Track time spent working on tasks.

### 📈 Productivity Analytics
- View task completion statistics.
- Monitor task distribution.
- Analyze productivity information.

### 🗄️ Database Integration
- Store task information in MongoDB.
- Use Mongoose for database operations.
- Maintain task data persistently.

### 🐳 Docker Containerization
- Run the Node.js application inside a Docker container.
- Run MongoDB as a separate container.
- Manage both services using Docker Compose.

---

## 🛠️ 3. Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive UI |
| JavaScript | Frontend interactions |
| Node.js | Backend runtime environment |
| Express.js | Server and REST API development |
| MongoDB | NoSQL database |
| Mongoose | MongoDB object data modeling |
| Docker | Application containerization |
| Docker Compose | Multi-container management |

---

## 🏗️ 4. System Architecture

TaskFlow follows a client-server architecture.

```text
                  USER
                    |
                    v
           FRONTEND INTERFACE
             HTML / CSS / JS
                    |
                    v
             EXPRESS SERVER
                Node.js
                    |
                    v
              MONGOOSE ODM
                    |
                    v
                MONGODB
                 DATABASE
```

### Docker Architecture

```text
             DOCKER COMPOSE
                    |
          +---------+---------+
          |                   |
          v                   v
     APP CONTAINER       MONGO CONTAINER
     Node.js +            MongoDB 7
     Express.js                |
          |                    |
          +--------------------+
              Docker Network
```

The frontend communicates with the Express backend through API requests. The backend uses Mongoose to interact with MongoDB and store task information.

Docker Compose manages the application and database as separate services.

---

## 📂 5. Project Structure

```text
TaskFlow/
│
├── public/
│   └── index.html
│
├── server.js
├── package.json
├── Dockerfile
├── docker-compose.yml
├── .dockerignore
├── .env.example
└── README.md
```

### File Description

| File | Description |
|---|---|
| `public/index.html` | Frontend interface |
| `server.js` | Express backend and API logic |
| `package.json` | Project dependencies and scripts |
| `Dockerfile` | Instructions to build the application image |
| `docker-compose.yml` | Configuration for application and MongoDB services |
| `.dockerignore` | Excludes unnecessary files from Docker builds |
| `.env.example` | Example environment configuration |
| `README.md` | Project documentation |

---

## ⚙️ 6. Installation and Execution

### Prerequisites

Make sure the following tools are installed:

- Node.js
- Docker Desktop
- Git

### Step 1: Clone the Repository

```bash
git clone https://github.com/GurvindapalliSriramcharan/task-manager-mongodb-docker.git
```

### Step 2: Navigate to the Project

```bash
cd task-manager-mongodb-docker
```

### Step 3: Build and Run Using Docker

```bash
docker compose up --build
```

This command builds the application image and starts the application and MongoDB services.

### Step 4: Open the Application

Open your browser and visit:

**http://localhost:3000**

### Step 5: Check Running Containers

```bash
docker compose ps
```

### Step 6: View Application Logs

```bash
docker logs task-manager-app
```

### Step 7: Stop the Application

```bash
docker compose down
```

---

## 🗄️ 7. Database Implementation

MongoDB is used as the database to store task information.

Mongoose provides schema-based data modeling and database interaction.

The application supports the following database operations:

- **Create:** Add a new task.
- **Read:** Retrieve existing tasks.
- **Update:** Modify task information and status.
- **Delete:** Remove tasks from the database.

The database runs as a separate Docker service. A named Docker volume is used for persistent database storage.

---

## 🐳 8. Docker Implementation

Docker is used to package the application and its dependencies into a container.

Docker Compose manages two services:

1. **Application Service:** Runs the Node.js and Express.js backend.
2. **MongoDB Service:** Runs the MongoDB database.

Both services communicate through the Docker network.

This approach provides:

- Consistent application execution.
- Simplified environment setup.
- Independent application and database services.
- Easier project portability.

---

## 📸 9. Application Highlights

The project demonstration includes:

- Main dashboard and task statistics.
- Creating and managing tasks.
- Kanban board with drag-and-drop functionality.
- Task time tracking.
- Productivity analytics.
- Backend implementation.
- MongoDB database connectivity.
- Docker container execution.

---

## 🎓 10. Learning Outcomes

Through this project, we gained practical experience in:

- Building interactive web applications.
- Developing backend services using Node.js and Express.js.
- Implementing CRUD operations.
- Connecting applications to MongoDB using Mongoose.
- Managing application dependencies.
- Containerizing applications using Docker.
- Running multi-container applications using Docker Compose.

---

## 🔮 11. Future Enhancements

Some possible future improvements include:

- User authentication and authorization.
- Multi-user task collaboration.
- Email and push notifications.
- Cloud deployment.
- Advanced productivity reports.
- Calendar integration.

---

## 🙌 Acknowledgement

This project was developed as part of **Web Programming – Assignment 2** to demonstrate the practical implementation of frontend development, backend development, database integration, and Docker containerization.

Thank you for reviewing our project!

---

<p align="center">
  <strong>TaskFlow – Plan Smart. Work Better. Achieve More. 🚀</strong>
</p>

<p align="center">
  Developed by <strong>G. Sriram Charan & Mahender Reddy</strong>
</p>
