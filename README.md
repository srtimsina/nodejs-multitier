# Multi-Tier Application with Node.js, React, and MongoDB

This is a multi-tier application that consists of a backend API built with Node.js, Express, and MongoDB, and a frontend client built with React. The application is containerized using Docker and managed using Docker Compose.

---

## Features

- **Backend**
  - RESTful API using Node.js and Express
  - MongoDB as the database for user management
  - Routes for fetching and creating users
  - Environment configuration using `dotenv`

- **Frontend**
  - React-based user interface
  - Axios for API calls
  - A form to add new users and display a list of users

- **Dockerized**
  - Separate Dockerfiles for backend and frontend
  - Docker Compose for multi-container orchestration

---

## Prerequisites

- **Node.js**: v18.x or higher
- **Docker**: Installed and running
- **MongoDB**: Used as the database (Dockerized)

---

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/srtimsina/nodejs-multitier.git
cd multi-tier-app
```

### 2. Set Up Environment Variables
Create a `.env` file in the `server` directory and add the following:

```bash
MONGO_URI=mongodb://database:27017/multiTierApp
PORT=5000
```

### 3. Build and Start Containers
Run the following command to build and start the application:

```bash
docker-compose up --build
```

### 4. Access the Application
- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:5000