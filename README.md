# MERN Stack App (Vite + React, Express, MongoDB)

## Structure

- `client/`: React app (Vite)
- `server/`: Express server (MongoDB ready)

## Usage

### 1. Start the server

```
cd server
npm install
npm start
```

Server runs on http://localhost:5000

### 2. Start the client

```
cd client
npm install
npm run dev
```

Client runs on http://localhost:5173 (default)

## Features

- Client fetches `/api/hello` from server and displays the message.

---

Replace MongoDB connection logic in `server/index.js` as needed for your database.

## Dockerized MERN Stack App

This app is fully dockerized using `docker-compose`.

### Quick Start

1. **Build and start all services:**

   ```bash
   docker-compose up --build
   ```

   - Client: http://localhost:3000
   - Server API: http://localhost:5000/api/hello
   - MongoDB: localhost:27017

2. **Stop all services:**
   ```bash
   docker-compose down
   ```

### Details

- `client/` and `server/` each have their own `Dockerfile`.
- MongoDB data is persisted in a Docker volume.
- The server connects to MongoDB using the `MONGO_URL` environment variable.

---

You can still run the client and server locally with npm if you prefer.
