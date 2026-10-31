# Fullstack JWT Authentication App

A full-stack application featuring advanced JWT authentication (Access and Refresh tokens).

## Tech Stack

**Frontend:**
*   React
*   TypeScript
*   MobX (State Management)
*   Axios (HTTP Client)

**Backend:**
*   Node.js
*   Express
*   MongoDB (Database)
*   JSON Web Tokens (JWT)
*   Nodemailer (Email verification)
*   Bcrypt (Password hashing)

**Infrastructure:**
*   Docker & Docker Compose (for database setup)

## Features
*   User registration with email verification.
*   User login (authentication).
*   User logout (with Refresh token invalidation).
*   Automatic Access token refresh (via Refresh token).
*   Protected routes (accessible only to authenticated users).

## How to Run Locally

### Prerequisites
Make sure you have the following installed:
*   [Node.js](https://nodejs.org/) (version 16+)
*   [Docker Desktop](https://www.docker.com/products/docker-desktop/)
*   Git

### Step 1: Clone the repository
```bash
git clone https://github.com/Haakkaa/Auth-App.git
cd Auth-App
```

### Step 2: Start the Database (Docker)
Navigate to the server folder (where docker-compose.yml is located) and run:
```bash
docker-compose up -d
```

### Step 3: Backend Setup
Navigate to the server folder (where docker-compose.yml is located) and run:

Navigate to the server directory:
```bash
cd server
```

Install dependencies:
```bash
npm install
```

Create a .env file based on .env.example:
```bash
cp .env.example .env
```

Start the server in development mode:
```bash
npm run dev
```

### Step 4: Frontend Setup

Open a new terminal and navigate to the client directory:
```bash
cd client
```

Install dependencies:
```bash
npm install
```

Start the React application:
```bash
npm start
```
The app will open in your browser at http://localhost:3000.
