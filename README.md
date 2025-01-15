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

## Project Structure

```
project-name/
├── client/          # Frontend application (React)
├── server/          # Backend application (Node.js, GraphQL, Prisma)
├── .env             # Environment variables
├── package.json     # Root dependencies
└── README.md        # Documentation
```

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

## Environment Variables

### Backend:
Create a `.env` file in the `server` folder with the following structure:

```env
DATABASE_URL="file:./dev.db"
PORT=4000
```

### Frontend:
Create a `.env` file in the `client` folder with the following structure:

```env
REACT_APP_GRAPHQL_ENDPOINT=http://localhost:4000/graphql
```

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request

---

## License

This project is licensed under the [MIT License](LICENSE).

