# Setup Guide

## Prerequisites

- Node.js v16+
- PostgreSQL 12+
- npm or yarn
- AWS Account (for media storage)

## Backend Setup

1. Navigate to backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create `.env` file from `.env.example`:
   ```bash
   cp .env.example .env
   ```

4. Update `.env` with your configuration:
   - Database connection string
   - JWT secret
   - AWS credentials
   - Email settings

5. Run database migrations:
   ```bash
   npm run migrate
   ```

6. Start the server:
   ```bash
   npm run dev
   ```

The server will run on `http://localhost:5000`

## Frontend Setup

1. Navigate to frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

The app will open at `http://localhost:3000`

## Database Setup

1. Create PostgreSQL database:
   ```bash
   createdb social_media
   ```

2. Run schema:
   ```bash
   psql social_media < database/schemas.sql
   ```

## AWS Configuration

1. Create an S3 bucket for media storage
2. Set up IAM user with S3 access
3. Add credentials to `.env` file
4. Configure bucket CORS policy for image uploads

## API Documentation

See `docs/API.md` for endpoint documentation.

## Troubleshooting

- **Port already in use**: Change PORT in `.env`
- **Database connection failed**: Check PostgreSQL is running and credentials in `.env`
- **AWS errors**: Verify AWS credentials and bucket name
