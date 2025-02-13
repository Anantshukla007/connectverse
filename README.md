# Connectverse & MelodyVerse Authentication System

## Overview
This project is a full-stack authentication system built using **React.js, Node.js, Express.js, PostgreSQL, and JWT**. It provides secure user authentication and registration for a fictional social media platform **Connectverse** on the backend while delivering visually appealing and user-friendly **login and signup screens** for a fictional music streaming service **MelodyVerse** on the frontend.

## Features
- Secure **JWT-based authentication**
- **User signup & login** with form validation
- Password **hashing with bcrypt** for security
- **React Router** for navigation
- **State management** using React hooks
- **Responsive design** with Tailwind CSS
- "Remember Me" functionality using **local storage**
- Basic **"Forgot Password"** functionality
- **Redirects** after authentication
- Error handling & validation messages
- Protects against **SQL Injection & XSS** attacks

## Bonus Features
- Password visibility toggle
- Basic email verification simulation on signup
- Rate limiting to prevent brute force attacks
- JWT authentication middleware
- Accessibility improvements (ARIA attributes, keyboard navigation)

---
## Tech Stack
### Frontend (React.js)
- **React 18** with Hooks
- **Tailwind CSS** for styling
- **React Router** for navigation
- **React Toastify** for notifications

### Backend (Node.js + Express)
- **Node.js** with Express.js
- **PostgreSQL** for database
- **JWT (jsonwebtoken)** for authentication
- **bcrypt** for password hashing
- **dotenv** for environment variables
- **express-rate-limit** for security

---
## Installation & Setup

### Prerequisites
Make sure you have **Node.js** and **PostgreSQL** installed on your system.

### Backend Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/connectverse-auth.git
   cd connectverse-auth
   ```
2. Install dependencies:
   ```sh
   cd backend
   npm install
   ```
3. Create a `.env` file in the `backend` directory:
   ```sh
   DATABASE_URL=your_database_url
   JWT_SECRET=your_jwt_secret
   PORT=5000
   ```
4. Run database migrations (PostgreSQL):
   ```sh
   npm run migrate
   ```
5. Start the backend server:
   ```sh
   npm start
   ```
   The API will run on `http://localhost:5000`

### Frontend Setup
1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the frontend server:
   ```sh
   npm start
   ```
   The app will be available at `http://localhost:3000`

---
## API Endpoints
### Authentication Routes
| Method | Route    | Description |
|--------|---------|-------------|
| POST   | /signup | Registers a new user |
| POST   | /login  | Logs in an existing user |

### Sample API Request (Signup)
```sh
POST /signup
{
  "username": "john_doe",
  "email": "john@example.com",
  "password": "StrongPassword123"
}
```

---
## Usage
1. **Signup** with a valid email and password.
2. **Login** using the registered credentials.
3. On successful login, you'll be redirected to the homepage.
4. Use the **Remember Me** feature to persist login sessions.

---
## Security Measures
- **Bcrypt** for secure password hashing
- **JWT tokens** for authentication & authorization
- **Rate limiting** to prevent brute force attacks
- **Input validation** to prevent SQL injection & XSS

---
## Future Enhancements
- Implement **password reset functionality**
- Add **2FA (Two-Factor Authentication)**
- Use **Redis for session management**
- Improve **UI animations with Framer Motion**

---
## Author
Developed by **Anant Shukla**

## License
This project is licensed under the **MIT License**

---


