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
