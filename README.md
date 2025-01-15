# Create React App with Prisma & GraphQL Backend

This project is a full-stack application built with **Create React App** for the client-side and a **Prisma** & **GraphQL** backend located in the `server` folder. The project demonstrates the integration of a modern front-end with a powerful back-end using GraphQL APIs.

---

## Table of Contents

- [Getting Started](#getting-started)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Scripts](#scripts)
- [Environment Variables](#environment-variables)
- [Contributing](#contributing)
- [License](#license)

---

## Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

Make sure you have the following tools installed on your system:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Docker](https://www.docker.com/) (optional for Prisma database)

---

## Technologies Used

### Frontend:
- React
- Apollo Client

### Backend:
- Node.js
- GraphQL
- Prisma ORM
- SQLite (default database, configurable)

---


---

## Backend Setup

1. Navigate to the `server` folder:

   ```bash
   cd server
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Configure Prisma:

   - Update the `prisma/schema.prisma` file to match your database configuration.

   - Run the following commands to set up the database:

     ```bash
     npx prisma migrate dev --name init
     npx prisma generate
     ```

4. Start the backend server:

   ```bash
   npm start
   ```

The backend server will run on `http://localhost:4000` by default.

---

## Frontend Setup

1. Navigate to the `client` folder:

   ```bash
   cd client
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the frontend application:

   ```bash
   npm start
   ```

The frontend application will run on `http://localhost:3000` by default.

---

## Scripts

### Root Scripts:

- `npm run client` - Starts the frontend application
- `npm run server` - Starts the backend application
- `npm run dev` - Runs both frontend and backend simultaneously (using `concurrently`)

### Backend Scripts:

- `npm start` - Starts the backend server
- `npx prisma migrate dev` - Runs database migrations
- `npx prisma studio` - Opens Prisma Studio to manage database

### Frontend Scripts:

- `npm start` - Starts the React development server
- `npm build` - Builds the React application for production

---
## App images

![Screenshot from 2025-01-15 20-39-36](https://github.com/user-attachments/assets/b5dc2cfc-d1d6-4e17-99d0-894e25aa7d77)
![Screenshot from 2025-01-15 20-39-25](https://github.com/user-attachments/assets/f7683325-dc86-4e68-a2b4-dd65173fdbf2)
![Screenshot from 2025-01-15 20-39-18](https://github.com/user-attachments/assets/10f6eb37-6cc8-485d-b123-efb1a58f7ee2)
![Screenshot from 2025-01-15 16-13-45](https://github.com/user-attachments/assets/75d4087b-7522-44af-953f-0ad59ece6f5e)
