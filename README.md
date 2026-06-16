# Hospital Management System

A full-stack, comprehensive web application designed to streamline hospital operations by providing dedicated portals for Patients, Doctors, and Administrators. This system handles everything from appointment booking to doctor management and user profiles.

---

## 🚀 Live Demo
- **Frontend**: [https://hospital-management-system-three-tau.vercel.app/](https://hospital-management-system-three-tau.vercel.app/)
- **Backend API**: Deployed on Render

---

## 🛠 Tech Stack

### Frontend
- **Framework**: React 19 with Vite
- **Styling**: Tailwind CSS
- **Routing**: React Router DOM
- **State Management**: React Context API
- **HTTP Client**: Axios
- **Notifications**: React Toastify

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JSON Web Tokens (JWT)
- **Image Storage**: Cloudinary (via Multer)
- **Security**: CORS, bcryptjs for password hashing

---

## ✨ Key Features

### 👨‍⚕️ For Patients (Users)
- **Authentication**: Secure Registration and Login.
- **Doctor Discovery**: Browse doctors by specialty, view their experience, fees, and availability.
- **Appointment Booking**: Schedule appointments with selected doctors.
- **Profile Management**: Update personal information, contact details, and profile picture.
- **My Appointments**: View upcoming appointments and cancel them if necessary.

### 🩺 For Doctors
- **Authentication**: Secure Login for doctors.
- **Doctor Dashboard**: Overview of earnings, total appointments, and recent patient activity.
- **Appointment Management**: View assigned appointments, mark them as completed, or cancel them.
- **Profile Customization**: Update availability, consultation fees, and professional details.

### 🛡️ For Administrators
- **Admin Dashboard**: Comprehensive view of hospital metrics (total doctors, patients, and appointments).
- **Manage Doctors**: Add new doctors to the system with their credentials, specialties, and images.
- **All Appointments**: View and manage all appointments across the entire hospital system.

---

## 📂 Project Structure

The repository is organized into a monorepo-style structure containing both the frontend and backend.

```
/
├── backend/                  # Node.js + Express API
│   ├── config/               # Database and Cloudinary configurations
│   ├── controllers/          # API logic for Auth, Users, Admin, Doctors
│   ├── middlewares/          # Auth verification and file upload middlewares
│   ├── models/               # MongoDB schemas (Mongoose)
│   ├── routes/               # API route definitions
│   └── server.js             # Entry point for the backend
│
└── frontend/                 # React + Vite Frontend
    ├── public/               # Static assets
    └── src/
        ├── assets/           # Images, icons, and static assets
        ├── components/       # Reusable React components
        ├── context/          # AppContext for global state management
        ├── pages/            # Application pages (Home, Login, Profile, etc.)
        └── main.jsx          # Entry point for the React application
```

---

## 💻 Local Development Setup

Follow these steps to run the project locally on your machine.

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Database (Local or MongoDB Atlas)
- Cloudinary Account (for image uploads)

### 1. Backend Setup
1. Open a terminal and navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Install the necessary dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `backend` folder and add your credentials:
   ```env
   PORT=4000
   MONGODB_URI=your_mongodb_connection_string
   CLOUDINARY_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   JWT_SECRET=your_secret_key
   ```
4. Start the backend development server:
   ```bash
   npm run dev
   ```

### 2. Frontend Setup
1. Open a new terminal window and navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install the necessary dependencies:
   ```bash
   npm install
   ```
3. Start the frontend Vite development server:
   ```bash
   npm run dev
   ```
4. The application should now be running locally, typically at `http://localhost:5173`.

---

## 🌍 Deployment

### Backend Deployment (Render)
1. Push your code to GitHub.
2. Create a new **Web Service** on [Render](https://render.com).
3. Connect your repository and set the **Root Directory** to `backend`.
4. Set the **Build Command** to `npm install`.
5. Set the **Start Command** to `npm start`.
6. Add your environment variables in the Render dashboard.
7. Deploy.

### Frontend Deployment (Vercel)
1. Create a new **Project** on [Vercel](https://vercel.com).
2. Connect your GitHub repository.
3. Edit the **Root Directory** to `frontend`.
4. Add an environment variable named `VITE_BACKEND_URL` and set its value to your newly deployed backend URL (e.g., `https://your-backend.onrender.com`).
5. Deploy.

---

## 📜 License
This project is licensed under the MIT License.
