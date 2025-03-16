<div align="center"> <img src="https://your-image-url-here.png" alt="ChatApp Logo" width="200"> <p>A modern, real-time chat platform built with the FARM stack</p>
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge(https://img.shields.io/badge/React-20232A?style=for-the-badge&ongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongocker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=whitroject Demo

<div align="center"> <table> <tr> <td align="center"><strong>Welcome</strong></td> <td align="center"><strong>Signup</strong></td> <td align="center"><strong>Login</strong></td> </tr> <tr> <td><img src="link-to-welcome-image" width="200"/></td> <td><img src="link-to-signup-image" width="200"/></td> <td><img src="link-to-login-image" width="200"/></td> </tr> <tr> <td align="center"><strong>API Docs</strong></td> <td align="center"><strong>Private Chat</strong></td> <td align="center"><strong>Group Chat</strong></td> </tr> <tr> <td><img src="link-to-api-docs-image" width="200"/></td> <td><img src="link-to-private-chat-image" width="200"/></td> <td><img src="link-to-group-chat-image" width="200"/></td> </tr> </table> </div>
✨ Features
<table> <tr> <td> <h3>📡 Real-time Communication</h3> <ul> <li>WebSocket integration for instant messaging</li> <li>Private and group chat functionality</li> <li>Message delivery status indicators</li> </ul> </td> <td> <h3>🔐 Secure Authentication</h3> <ul> <li>JWT-based authentication system</li> <li>Email verification process</li> <li>Password encryption with Passlib</li> </ul> </td> </tr> <tr> <td> <h3>🛡️ Robust Validation</h3> <ul> <li>Client-side form validation</li> <li>Server-side data validation with Pydantic</li> <li>Input sanitization for security</li> </ul> </td> <td> <h3>🐳 Containerized Setup</h3> <ul> <li>Docker configuration for backend</li> <li>Docker configuration for frontend</li> <li>Easy deployment with docker-compose</li> </ul> </td> </tr> </table>
🔧 Technology Stack
Frontend
React: A powerful JavaScript library for building user interfaces

Vite: Modern development environment that optimizes frontend development

Axios: Promise-based HTTP client for API requests

Framer Motion: Animation library for React

React Router: Declarative routing for React applications

Websocket Client: For real-time communication

Tailwind CSS: Utility-first CSS framework

Backend
FastAPI: Modern Python framework for efficient API development

Pydantic: Data validation and settings management

Motor & PyMongo: MongoDB async driver and tools

WebSockets: Real-time chat implementation

Cryptography & Passlib: Security for user data

Celery: Asynchronous task processing (email verification)

Uvicorn: ASGI server for FastAPI

🚀 Getting Started
Prerequisites
Node.js and npm

Python 3.7+ and pip

MongoDB server

Redis (for Celery tasks)

Quick Setup
Clone Repository

bash
git clone https://github.com/rhsajib/real-time-chat-app.git
cd real-time-chat-app
Backend Setup

bash
cd chatp-root/backend/app
# Configure environment variables according to .env.demo
cd ..
pip install -r requirements.txt
uvicorn app.main:app --reload
Your FastAPI server should now be running on http://localhost:8000

Frontend Setup

bash
cd chatp-root/frontend
# Configure environment variables according to .env.demo
npm install
npm run dev
Your React development server should now be running on http://localhost:8080

Celery Setup

bash
cd chatp-root/backend
celery -A app.services.worker.celery.celery worker --loglevel=info
🐳 Docker Setup
For a containerized environment:

bash
cd chatp-root
# Configure environment variables first
docker-compose up --build
The backend will be accessible at http://localhost:8000 and the frontend at http://localhost:8080.

📝 Usage Instructions
First-time Setup:

Create multiple user accounts with unique email addresses

Verify email addresses to activate accounts

Starting Conversations:

After creating accounts, you can find other users in the sidebar

Start private conversations or create group chats

Experience real-time messaging with instant delivery

Exploring Features:

Try out the real-time chat functionality

Test the authentication system

Explore private and group messaging capabilities

📜 License
This project is licensed under the MIT License - see the LICENSE.md file for details.

<div align="center">
