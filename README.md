# Basic Backend API

A simple Node.js API for user registration and login.

## Setup

1. Install dependencies:
   ```
   npm install
   ```

2. Start the server:
   ```
   npm start
   ```

   For development with auto-restart:
   ```
   npm run dev
   ```

## API Endpoints

### Register User
- **POST** `/api/auth/register`
- Body: `{ "email": "user@example.com", "password": "password123" }`
- Response: `{ "message": "User registered successfully" }`

### Login User
- **POST** `/api/auth/login`
- Body: `{ "email": "user@example.com", "password": "password123" }`
- Response: `{ "token": "jwt_token_here" }`

## Notes
- Users are stored in `users.json` (not suitable for production).
- JWT secret is hardcoded as 'secretkey' (change for production).
- No input validation beyond basic checks.