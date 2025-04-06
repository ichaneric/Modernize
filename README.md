# Modernize Full-Stack Application

This repository contains a full-stack application with a React Next.js frontend and an Express.js backend API.

## Project Structure

- **cctc-demo-backend-section-a**: Express.js backend API with PostgreSQL database
- **Modernize-Nextjs-Free**: Next.js frontend application with Material UI

## Prerequisites

Before setting up the project, ensure you have the following installed:

- **Node.js** (v16 or higher recommended)
- **npm** (included with Node.js)
- **PostgreSQL** database server

You can verify your installations by running:
```bash
node -v
npm -v
```

## Backend Setup (Express.js API)

### 1. Navigate to the backend directory
```bash
cd cctc-demo-backend-section-a
```

### 2. Install dependencies
```bash
npm install
```

### 3. Configure environment variables
Create or update the `.env` file with the following variables:
```
PORT=5000
DB_USER=your_postgres_username
DB_PASSWORD=your_postgres_password
DB_NAME=cctc-demo-section-a
DB_HOST=localhost
JWT_SECRET=your_jwt_secret_key
```

### 4. Database setup
Create a PostgreSQL database named `cctc-demo-section-a` (or as specified in your .env)

### 5. Run database migrations
```bash
npx sequelize-cli db:migrate
```

### 6. Start the backend server
```bash
node server.js
```

The API will be available at: http://localhost:5000

## Frontend Setup (Next.js)

### 1. Navigate to the frontend package directory
```bash
cd Modernize-Nextjs-Free/package
```

### 2. Install dependencies
```bash
npm install
```

### 3. Start the development server
```bash
npm run dev
```

The frontend application will be available at: http://localhost:3000

### 4. Build for production
```bash
npm run build
```

### 5. Start the production server
```bash
npm start
```

## API Documentation

The backend provides the following endpoints:

- User authentication: `/api/users/login`
- User registration: `/api/users/register`
- Additional endpoints are documented in the API routes

## Technologies Used

### Backend
- Express.js - Web application framework
- Sequelize - ORM for database operations
- PostgreSQL - Database
- JWT - Authentication
- Bcrypt.js - Password hashing

### Frontend
- Next.js 14 - React framework
- Material UI - Component library
- TypeScript - Type safety
- Apex Charts - Data visualization

## Troubleshooting

If you encounter any issues setting up the project:

1. Ensure PostgreSQL is running
2. Check database credentials in the .env file
3. Make sure all dependencies are installed
4. Verify Node.js version compatibility

## License

This project is licensed under the terms specified in the LICENSE file. 
