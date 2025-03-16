# Real Time Chat Application (FARM Stack Project)

This FARM (FastAPI, React, and MongoDB) project is a full-stack web application that combines the power of **FastAPI** for the backend, **React** for the frontend, and **MongoDB** for data storage. It features JWT authentication, email verification, real-time chat using **WebSockets**, and more.

## Table of Contents
- [Features](#features)
- [Frontend](#frontend)
- [Backend](#backend)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Clone or Download Repository](#explore-chatp)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
  - [Celery Setup](#celery-setup)
  - [Redis & Database Configuration](#redis-configuration)
  - [Docker Setup](#docker-setup)
- [Usage Instructions](#usage-instructions)
- [License](#license)

## Features

- **FastAPI Backend**: Provides RESTful API endpoints.
- **React Frontend**: A user-friendly interface for chatting in real-time.
- **MongoDB Database**: Efficient data storage for users and messages.
- **JWT Authentication**: Secure user access and session management.
- **Email Verification**: Ensures that users verify their email addresses.
- **Field Validation**: Ensures data integrity on both the client and server side.
- **WebSocket Integration**: Real-time chat functionality with WebSockets.
- **Separate Collections**: Distinct MongoDB collections for private and group chat.
- **Docker Setup**: Containerized development environment for both frontend and backend.

## Frontend

The frontend of the Real Time Chat Application is built using **React** and **Vite** for a fast development experience. Key technologies include:

- **React**: A powerful JavaScript library for building user interfaces.
- **Vite**: A modern development environment for React.
- **Dependencies**: Axios, Framer Motion, React Router, WebSocket Client for efficient communication.
- **DevDependencies**: ESLint and Tailwind CSS for code quality and styling.

The frontend integrates client-side authentication to ensure only authorized users can access chat features.

## Backend

Our backend, powered by **FastAPI**, includes the following components:

- **FastAPI**: A modern Python framework for high-performance API development.
- **Pydantic**: For data validation and settings management.
- **Motor and PyMongo**: MongoDB support for database operations.
- **WebSockets**: For real-time communication via WebSocket integration (python-socketio and starlette).
- **Cryptography and Passlib**: For secure password storage and encryption.
- **Celery**: Asynchronous task processing for email verification and more.

## Getting Started

### Prerequisites
Before you begin, ensure you have the following installed:

- **Node.js** and **npm** for React + Vite development.
- **Python** and **pip** for FastAPI development.
- **MongoDB** server running locally or using a cloud-based service.
- **Redis** for Celery task queue.

### Explore 

1. **Clone or Download Repository**
   ```bash
   git clone https://github.com/rhsajib/real-time-chat-app.git
   cd real-time-chat-app

Backend Setup
Environment Variable Setup:

Navigate to the backend folder:
bash
Copy
cd backend/app
Follow the steps in the .env.demo file to set environment variables.
Install Dependencies:

bash
Copy
pip install -r requirements.txt
Run the FastAPI Backend:

bash
Copy
uvicorn app.main:app --reload
Your FastAPI server will be running at http://localhost:8000.

Frontend Setup
Environment Variable Setup:

Navigate to the frontend folder:
bash
Copy
cd frontend
Follow the steps in the .env.demo file to set environment variables.
Install Dependencies:

bash
Copy
npm install
Start the React Development Server:

bash
Copy
npm run dev
Your frontend will be available at http://localhost:8080.

Celery Setup
Start the Celery Worker:
bash
Copy
cd backend
celery -A app.services.worker.celery.celery worker --loglevel=info
Redis Configuration
Set up Redis in the backend to manage Celery task queues.

Database Configuration
Ensure MongoDB is running and set up your connection in the backend.

Docker Setup
To containerize the application with Docker:

Build and Start the Containers:

bash
Copy
cd real-time-chat-app
docker-compose up --build
This will start both the backend and frontend containers.

Backend: http://localhost:8000
Frontend: http://localhost:8080
Usage Instructions
Initialization
When you first launch the application, the database will be empty. You need to create user accounts with unique email addresses. This is a one-time setup.

Creating User Accounts
Start by creating user profiles with distinct email addresses to avoid validation errors.

Engaging in Conversations
Once multiple users are registered, you can engage in real-time chat. The Users section from the sidebar will display all available users, and you can initiate chats with them.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.


