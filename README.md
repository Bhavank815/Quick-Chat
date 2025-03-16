Real Time Chat Application (FARM Stack)
<div align="center"> <img src="https://your-logo-url-here.png" alt="Chat Application Logo" width="150"> <p>A modern, real-time chat platform built with the FARM stack</p>
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?stylct](https://img.shields.io/badge/React-20232A?style=for-the-badgeongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=whg.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=whiteatures

Real-time Communication: WebSocket integration for instant messaging

JWT Authentication: Secure user access and data protection

Email Verification: Required verification for account activation

Comprehensive Validation: Both client-side and server-side validation

Private & Group Chats: Separate collections for different chat types

Containerized Setup: Docker configurations for easy deployment

🛠️ Tech Stack
Frontend
React: User interface library

Vite: Frontend build tool

Axios: HTTP client for API requests

Framer Motion: Animation library

React Router: Application routing

Websocket Client: Real-time communication

Tailwind CSS: Styling framework

Backend
FastAPI: Python web framework

Pydantic: Data validation

Motor & PyMongo: MongoDB interaction

WebSockets: Real-time functionality

Cryptography & Passlib: Security tools

Celery: Async task processing

Uvicorn: ASGI server

🚀 Getting Started
Prerequisites
Node.js and npm

Python 3.7+ and pip

MongoDB server

Redis server (for Celery)

Installation
Clone Repository
bash
git clone https://github.com/rhsajib/real-time-chat-app.git
cd real-time-chat-app
Backend Setup
bash
# Navigate to backend directory
cd chatp-root/backend/app

# Configure environment variables (see .env.demo file)
# Then return to backend root
cd ..

# Install dependencies
pip install -r requirements.txt

# Start FastAPI server
uvicorn app.main:app --reload
Frontend Setup
bash
# Navigate to frontend directory
cd chatp-root/frontend

# Configure environment variables (see .env.demo file)

# Install dependencies
npm install

# Start development server
npm run dev
Celery Setup
bash
cd chatp-root/backend
celery -A app.services.worker.celery.celery worker --loglevel=info
Docker Setup
bash
# Navigate to root directory
cd chatp-root

# Configure environment variables first
# Then build and start containers
docker-compose up --build
The backend will be accessible at http://localhost:8000 and the frontend at http://localhost:8080.

📝 Usage
Initial Setup:

Create multiple user accounts with unique email addresses

Verify your email to activate your account

Chat Functionality:

Find users in the sidebar

Start private conversations

Create or join group chats

Experience real-time messaging

🧪 API Documentation
FastAPI provides automatic interactive API documentation. Once the server is running, visit:

Swagger UI: http://localhost:8000/docs

ReDoc: http://localhost:8000/redoc

🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Fork the repository

Create your feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add some amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE.md file for details.
