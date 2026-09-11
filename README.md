# MERN Social Platform

A full-stack social application built with MongoDB, Express, React, and Node.js. The project covers the core pieces of a modern authenticated web app: user registration and login, protected routes, profile pages, posts, image uploads, persistent client state, and a responsive Material UI interface.

## What this project demonstrates

- React 18 application structure with protected routing
- Redux Toolkit and `redux-persist` for client-side state
- Formik + Yup for form handling and validation
- Material UI theming, including light/dark mode support
- Node.js / Express REST API
- MongoDB / Mongoose data models
- JWT-based authentication and protected API routes
- Password hashing with bcrypt
- Image uploads with Multer
- Basic API hardening with Helmet, CORS, and request logging

## Tech stack

**Frontend**
- React
- Redux Toolkit
- React Router
- Material UI
- Formik / Yup

**Backend**
- Node.js
- Express
- MongoDB / Mongoose
- JWT
- bcrypt
- Multer
- Helmet

## Project structure

```text
.
├── client/             # React frontend
│   ├── public/
│   └── src/
│       ├── components/
│       ├── scenes/
│       └── state/
└── server/             # Express API
    ├── controllers/
    ├── middleware/
    ├── models/
    ├── routes/
    └── public/
```

## Running locally

### 1. Configure the backend

Copy the example environment file:

```bash
cp server/.env.example server/.env
```

Then add your local values:

```env
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=3001
```

### 2. Start the server

```bash
cd server
npm install
npm start
```

### 3. Start the client

In a second terminal:

```bash
cd client
npm install
npm start
```

## Notes

This repository is one of my full-stack application projects and reflects the way I approach application work across both the UI and API layers. I tend to focus on practical architecture, clear user flows, and making the frontend and backend fit together cleanly rather than treating them as separate problems.
