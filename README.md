<<<<<<< HEAD
# Task Manager — MongoDB + Docker

A small course project built with **Node.js, Express, MongoDB, Mongoose and Docker Compose**.

## Features
- Add a task
- View all saved tasks
- Mark tasks complete/incomplete
- Delete tasks
- Persist data in MongoDB using a Docker volume

## Run with Docker (recommended)
1. Install and start Docker Desktop.
2. Extract this project folder.
3. Open a terminal in this folder.
4. Run:

   ```bash
   docker compose up --build
   ```

5. Open http://localhost:3000

To stop: press `Ctrl + C`, then run `docker compose down`.
To stop and also delete saved database data: `docker compose down -v`.

## Run without Docker (optional)
1. Install Node.js and MongoDB.
2. Run `npm install`.
3. Copy `.env.example` to `.env`.
4. Ensure MongoDB is running locally.
5. Run `npm start`.
6. Open http://localhost:3000

## API endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/tasks` | Get all tasks |
| POST | `/api/tasks` | Create a task; JSON: `{"title":"Finish assignment"}` |
| PATCH | `/api/tasks/:id` | Update completion; JSON: `{"completed":true}` |
| DELETE | `/api/tasks/:id` | Delete a task |

## How Docker is used
- `Dockerfile` packages the Node.js application into an image.
- `docker-compose.yml` starts the application and MongoDB as separate containers.
- The app connects to MongoDB using the service name `mongo` on Docker's internal network.
- `mongo_data` is a named volume, so database data remains after containers stop.

## Database
Database: `taskmanager`  
Collection: `tasks`  
Fields: `_id`, `title`, `completed`, `createdAt`, `updatedAt`

## 1-minute demonstration
1. Open the app.
2. Add two tasks.
3. Mark one as completed.
4. Delete one task.
5. Refresh the page to show that remaining tasks persist in MongoDB.

## Project abstract
The Task Manager is a simple web application that helps users maintain a list of daily activities. It provides create, read, update and delete (CRUD) operations through a REST API. MongoDB stores task records, while Docker and Docker Compose containerize the application and database, making the project easy to run consistently across different systems.
=======
# task-manager-mongodb-docker
>>>>>>> ce8cd49605102df933d3e003ea83c158da95755d
