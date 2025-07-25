# AppointMe

AppointMe is a full-stack appointment booking platform for users and doctors, built with Node.js, Express, MongoDB, and React.  
It supports user registration, login, doctor management, appointment booking/cancellation, and admin features.

---

## Features

- **User Registration & Login** (JWT-based authentication)
- **Doctor Registration & Login**
- **Admin Panel** for managing doctors and appointments
- **Book & Cancel Appointments**
- **User & Doctor Profile Management**
- **Protected Routes** using authentication middleware
- **Cloudinary** for profile image uploads
- **MongoDB** for data storage

---

## Tech Stack

- **Frontend:** React, Axios
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT
- **File Uploads:** Cloudinary
- **Password Hashing:** bcrypt

---

## Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/yourusername/AppointMe.git
cd AppointMe
```

### 2. Install dependencies

#### Backend
```sh
cd backend
npm install
```

#### Frontend
```sh
cd ../frontend
npm install
```

### 3. Set up environment variables

Create a `.env` file in the `backend` directory:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
```

### 4. Start the servers

#### Backend
```sh
cd backend
npm start
```

#### Frontend
```sh
cd ../frontend
npm start
```

---

## Folder Structure

```
AppointMe/
  backend/
    controllers/
    middlewares/
    models/
    routes/
    .env
    server.js
  frontend/
    src/
    public/
    package.json
```

---

## API Overview

- **User:** `/api/user/register`, `/api/user/login`, `/api/user/profile`, `/api/user/appointments`
- **Doctor:** `/api/doctor/register`, `/api/doctor/login`, `/api/doctor/profile`, `/api/doctor/appointments`
- **Admin:** `/api/admin/login`, `/api/admin/doctors`, `/api/admin/appointments`

---

## Notes

- All sensitive data (like JWT secrets and DB URIs) should be stored in `.env` files (see `.gitignore`).
- Make sure MongoDB and Cloudinary credentials are correct.
- Use valid MongoDB ObjectIds for all database references.

---

## License
