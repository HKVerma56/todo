

# To-Do Application

This project is a full-stack to-do application built using .NET 8 for the Web API, MongoDB for data storage, and Angular for the frontend.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Frontend](#frontend)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Task Management:** Create, update, delete, and view tasks.
- **User Authentication:** Secure access to the application with JWT-based authentication.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Technologies Used

- **Backend:**
  - .NET 8 (Web API)
  - MongoDB (Database)
  - JWT for Authentication

- **Frontend:**
  - Angular
  - Angular Material (for UI components)

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Node.js and npm](https://nodejs.org/en/download/)
- [MongoDB](https://www.mongodb.com/try/download/community)

### Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/HKVerma56/todo.git]
   cd todo
   ```

2. **Backend Setup:**

   - Navigate to the `backend` directory:
     ```bash
     cd backend
     ```

   - Install the required packages:
     ```bash
     dotnet restore
     ```

   - Set up your MongoDB connection string in `appsettings.json`:
     ```json
     "ConnectionStrings": {
       "MongoDb": "your-mongodb-connection-string"
     }
     ```

   - Run the application:
     ```bash
     dotnet run
     ```

3. **Frontend Setup:**

   - Navigate to the `frontend` directory:
     ```bash
     cd ../frontend
     ```

   - Install the required packages:
     ```bash
     npm install
     ```

   - Run the Angular development server:
     ```bash
     ng serve
     ```

4. **Access the application:**
   - Backend API will be running at `https://localhost:5001`.
   - Frontend will be running at `http://localhost:4200`.

## API Endpoints

### Task Endpoints

- **GET /api/tasks:** Retrieve all tasks
- **GET /api/tasks/{id}:** Retrieve a task by ID
- **POST /api/tasks:** Create a new task
- **PUT /api/tasks/{id}:** Update a task
- **DELETE /api/tasks/{id}:** Delete a task

### Authentication Endpoints

- **POST /api/auth/register:** Register a new user
- **POST /api/auth/login:** Login a user and retrieve a JWT

## Frontend

The frontend is built using Angular and includes components for managing tasks and user authentication.

- **Task List Component:** Displays the list of tasks.
- **Task Form Component:** Allows users to create and edit tasks.
- **Login and Register Components:** Handle user authentication.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

