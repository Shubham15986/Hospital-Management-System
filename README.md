# Hospital Management System

A comprehensive web application for managing hospital operations, including patient and doctor interactions, profiles, and administrative tasks.

## Tech Stack
- **Frontend**: React, Vite, Tailwind CSS, Axios, Context API
- **Backend**: Node.js, Express.js, MongoDB, JWT for authentication, Cloudinary for image storage

## Project Structure
- `/frontend` - Contains the React Vite application.
- `/backend` - Contains the Node.js Express API.

## Features
- **Patient Portal**: Patients can view doctors, book appointments, and manage their profiles.
- **Doctor Portal**: Doctors can view their appointments and manage their profiles.
- **Admin Portal**: Administrators can manage doctors, patients, and system settings.
- **Authentication**: Secure login and signup with JWT tokens.

## Local Development Setup

### 1. Backend Setup
1. Navigate to the `backend` directory: `cd backend`
2. Install dependencies: `npm install`
3. Create a `.env` file with your credentials (e.g., MongoDB URI, Cloudinary keys, JWT Secret).
4. Start the server: `npm run dev` (for development) or `npm start` (for production)

### 2. Frontend Setup
1. Navigate to the `frontend` directory: `cd frontend`
2. Install dependencies: `npm install`
3. Start the application: `npm run dev`

## Deployment
The backend can be deployed easily on platforms like Render by setting the build command to `npm install` and the start command to `npm start`.
The frontend can be deployed on Vercel or Netlify by providing the `VITE_BACKEND_URL` environment variable pointing to the deployed backend URL.

## License
MIT
