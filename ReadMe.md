# Polling App

## Introduction
A full-stack polling app with real-time voting results. Built using React, Node.js, Express, and MySQL, with Docker for containerization and deployed on AWS EC2.

## Features
- Create and manage polls
- Vote on polls with real-time updates
- User authentication (Signup/Login)
- Responsive UI with React
- MySQL database integration
- Dockerized setup
- Hosted on AWS EC2

## Tech Stack
- **Frontend**: React, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Containerization**: Docker
- **Real-time Communication**: Socket.io
- **Deployment**: AWS EC2, Nginx

## Setup
### Prerequisites
- Node.js & npm
- MySQL
- Docker
- AWS account (for deployment)

### Backend Setup
```sh
cd backend
npm install
cp .env.example .env  # Configure DB credentials
npm start
```

### Frontend Setup
```sh
cd frontend
npm install
npm start
```

### Docker Setup
```sh
docker-compose up --build
```

## API Endpoints
- `POST /api/auth/register` - Register user
- `POST /api/auth/login` - Login user
- `POST /api/polls` - Create poll
- `GET /api/polls` - Get all polls
- `POST /api/polls/:id/vote` - Vote on poll

## Deployment on AWS EC2
1. Launch an EC2 instance
2. Install Docker & Docker Compose
3. Clone repo & run `docker-compose up -d`
4. Configure Nginx as a reverse proxy

## Future Improvements
- OAuth login (Google, GitHub)
- Unit & integration tests
- Kubernetes deployment


