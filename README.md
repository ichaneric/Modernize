# Modernize - Full-Stack Project

A full-stack application integrating a Next.js frontend with an Express.js API, built to demonstrate user registration, login, and adding users/products with JWT authentication.

## Project Structure
- `Modernize-Nextjs-Free/`: Frontend built with Next.js (UI for register, login, and add functionality).
- `cctc-demo-backend-section-a/`: Backend built with Express.js (API endpoints).
- `branches-screenshot.png`: Screenshot of GitHub branches for submission.

## Setup Instructions

### Prerequisites
- Node.js (v16 or higher)
- npm
- Git

### 1. Clone the Repository
```bash
git clone https://github.com/ichaneric/Modernize.git
cd Modernize
2. Backend Setup
Install dependencies and start the Express.js server:

bash

Collapse

Wrap

Copy
cd cctc-demo-backend-section-a
npm install
npm start
The backend should run on http://localhost:3000 (adjust port if customized).
#### 3. Frontend Setup
Install dependencies and start the Next.js app:

bash

Collapse

Wrap

Copy
cd Modernize-Nextjs-Free
npm install
npm run dev
The frontend should run on http://localhost:3001 (or Next.js default 3000—adjust if there’s a conflict).
### 4. API Endpoints
Register: POST /api/users/register
Example: { "username": "test", "password": "pass123" }
Login: POST /api/users/login
Example: { "username": "test", "password": "pass123" }
Returns a JWT token stored in localStorage.
Add User: POST /add-user (protected route)
Requires JWT token in Authorization header: Bearer <token>.
5. Usage
Open your browser to the frontend URL (e.g., http://localhost:3001).
Use the UI to register, log in, and add a user/product, with success/failure messages displayed.
Git Flow
Branches: main, development, feature/register, feature/login, feature/add-user.
See branches-screenshot.png for branch structure.
Reflection
