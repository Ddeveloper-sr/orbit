# Orbit Full Stack v1.0

A Discord-inspired communication app built with React/Vite, Node/Express, JWT authentication, JSON persistence, and Socket.IO real-time messaging.

## Local development

```bash
npm install
cp .env.example .env
npm run dev
```

Client: `http://localhost:5173`
API: `http://localhost:3001`

## Structure

- `client/` — React + Vite frontend
- `server/` — Express + Socket.IO backend
- `.env.example` — environment template

## Important deployment note

The Vite frontend can be deployed to Vercel. The current Express + Socket.IO backend requires a long-running Node.js host and should not be deployed as a Vercel serverless function without refactoring the realtime architecture.

Do not commit `.env` or production secrets.
