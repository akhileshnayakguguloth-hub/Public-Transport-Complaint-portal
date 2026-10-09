# Public Transport Complaint Portal

MERN application for reporting and managing public transport complaints.

## Features
- Passenger registration/login (bcrypt password hashing and JWT sessions)
- Role-based passenger/admin access
- Complaint creation, tracking, history, filters and status updates
- Admin CRUD for buses, routes and locations; dashboard statistics
- Responsive React UI, API validation, rate limiting, security headers and error handling

## Requirements
Node.js 20+ and MongoDB (local or Atlas).

## Run
1. Copy `server/.env.example` to `server/.env`; set a random `JWT_SECRET` (32+ characters) and `MONGO_URI`.
2. Run `npm install`, then `npm run install:all`.
3. Run `npm run dev`; open http://localhost:5173. API health: http://localhost:5000/api/health.
4. Register a user, then promote that account to `role: "admin"` in MongoDB. Public admin registration is intentionally disabled.

## Scripts
`npm run dev` starts API and UI; `npm run build` builds the frontend; `npm start` starts API.
