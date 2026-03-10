💬 Chatterly Backend

🚀 Chatterly Backend is a scalable backend service powering the Chatterly communication platform, developed by Stackly Engineering Team.
It supports secure authentication, real-time messaging, chat services, and scalable API architecture.

📌 Table of Contents

1. Project Overview
2. Tech Stack
3. System Architecture
4. Project Structure
5. Installation
6. Environment Setup
7. API Structure
8. Git Workflow
9. Security Rules
10. Contributors
11. Future Improvements

📖 Project Overview

Chatterly is a modern communication platform built to support:

✔ Secure User Authentication
✔ Real-Time Chat Messaging
✔ Chat Room Management
✔ Scalable Backend APIs
✔ Secure Token Authentication
✔ WebSocket Communication

This backend system is designed to support high scalability and production deployment.

🛠 Tech Stack
Technology	Usage
Node.js	Backend runtime
Express.js	API framework
MongoDB	Database
Mongoose	ODM
Socket.IO	Real-time messaging
JWT	Authentication
bcrypt	Password hashing
dotenv	Environment configuration
Morgan	API logging
Helmet	Security headers

🏗 System Architecture
Client (Web / Mobile)
        │
        │ HTTP / WebSocket
        ▼
Express API Server
        │
        │
        ▼
Application Layer
Controllers → Services → Middleware
        │
        ▼
MongoDB Database

Real-time communication handled via:

Socket.IO Server
     │
     ▼
Live Chat Messaging
Online User Tracking
Notifications

📂 Project Structure
Chatterly_backend
│
├── src
│   ├── config          # Database & environment configs
│   ├── controllers     # API request handlers
│   ├── middleware      # Auth & security middleware
│   ├── models          # Database models
│   ├── routes          # API route definitions
│   ├── services        # Business logic
│   ├── utils           # Helper utilities
│
├── tests               # Unit tests
├── docs                # API documentation
│
├── server.js           # Application entry point
├── package.json
├── .env.example
└── README.md

⚙ Installation
1️⃣ Clone Repository
git clone https://github.com/BHARATHWAJ113/Chatterly_backend.git
2️⃣ Navigate to project
cd Chatterly_backend
3️⃣ Install Dependencies
npm install
4️⃣ Run Development Server
npm run dev
5️⃣ Production Run
npm start
🔐 Environment Setup

Create .env file in root folder.

Example configuration:

PORT=5000
MONGO_URI=mongodb://localhost:27017/chatterly
JWT_SECRET=your_super_secret_key

🌐 API Base URL
http://localhost:5000/api

Example endpoint:

POST /api/auth/login
POST /api/auth/register
GET  /api/users
POST /api/messages

🌿 Git Workflow

We follow a controlled Git branching strategy.

Branch	Purpose
main	Production
develop	Integration
feature/*	Feature development
hotfix/*	Emergency fixes

Example:

feature/login-api
feature/chat-module

👨‍💻 Developer Workflow

1. Pull latest code
git pull origin develop
2. Create feature branch
git checkout -b feature/new-feature
3. Commit changes
git commit -m "Added login API"
4. Push branch
git push origin feature/new-feature
5. Create Pull Request
PR must be merged into develop branch first.

🔒 Security Rules

✔ Direct push to main branch disabled
✔ All merges require Pull Request approval
✔ Environment variables stored in .env
✔ .env file excluded from Git

👥 Contributors
Name	Role
Cipher Squad	Development Team


🚀 Future Improvements

- Planned enhancements:
- Redis caching
- API rate limiting
- Microservices architecture
- Docker deployment
- Kubernetes scaling
- CI/CD automation
- Swagger API documentation
- Notification service
- Media upload system

🏢 Developed By

Stackly Cipher Squad

📜 License

MIT License