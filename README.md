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




