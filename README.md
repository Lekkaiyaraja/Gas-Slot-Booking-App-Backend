# FuelOne Gas Slot Booking - Backend

Welcome to the **FuelOne Gas Slot Booking Backend**, a robust and scalable backend system designed to handle gas slot bookings, user authentication, payment processing, and notifications. This backend provides a seamless API for managing gas deliveries efficiently.

## 📌 Overview

The **FuelOne Gas Slot Booking Backend** is built using **Node.js** and **Express.js**, leveraging **MongoDB** for data storage. It supports user authentication, secure payment processing via Razorpay, and real-time booking management.

## 🚀 Features

- **User Authentication** (JWT-based secure authentication)
- **Gas Slot Booking** (Users can select and book available slots)
- **Payment Integration** (Razorpay payment gateway for seamless transactions)
- **Email Notifications** (Order confirmations & payment status updates)
- **Admin Controls** (Manage bookings and payment verifications)
- **Error Handling & Security** (Protected API routes with proper error handling)

---

## 💂️ Project Structure

```
FuelOne-Backend/
│—— controllers/
│   ├— userController.js   # Handles user authentication and profile
│   ├— bookingController.js # Manages slot bookings and payments
│—— routes/
│   ├— userRoutes.js      # Routes for user authentication
│   ├— bookingRoutes.js   # Routes for booking operations
│—— models/
│   ├— userSchema.js      # MongoDB schema for users
│   ├— bookingSchema.js   # MongoDB schema for gas slot bookings
│—— config/
│   ├— database.js        # MongoDB connection configuration
│—— middleware/
│   ├— authMiddleware.js  # JWT authentication middleware
│—— utils/
│   ├— emailService.js    # Nodemailer email integration
│—— .env                   # Environment variables for sensitive data
│—— server.js              # Main application entry point
│—— package.json           # Project dependencies and scripts
```

---

## 🛠️ Technologies Used

- **Node.js** - JavaScript runtime for backend
- **Express.js** - Web framework for building RESTful APIs
- **MongoDB & Mongoose** - NoSQL database for storing users and bookings
- **JWT (jsonwebtoken)** - Secure user authentication
- **Razorpay** - Payment gateway for handling transactions
- **Nodemailer** - Email service for order confirmations
- **dotenv** - Environment variable management
- **bcryptjs** - Secure password hashing
- **cors** - Cross-Origin Resource Sharing for API access control

---

## 📌 API Endpoints

| **Route**                 | **Method** | **Endpoint**             | **Description**                              |
|-------------------------- |-----------|--------------------------|----------------------------------------------|
| **User Registration**      | `POST`    | `/api/register`          | Registers a new user with secure hashing.  |
| **User Login**             | `POST`    | `/api/login`             | Authenticates user and returns JWT token.  |
| **Book Gas Slot**          | `POST`    | `/api/book-slot`         | Books a slot for gas delivery.             |
| **Get User Bookings**      | `GET`     | `/api/user/bookings`     | Fetches booking history for a user.        |
| **Update Payment Status**  | `POST`    | `/api/payment-update`    | Updates payment status after transaction.  |

---

## 🛠️ Setup Instructions

### 1️⃣ Clone Repository
```sh
git clone https://github.com/Lekkaiyaraja/Gas-Slot-Booking-App-Backend.git
cd Gas-Slot-Booking-App-Backend
```

### 2️⃣ Install Dependencies
```sh
npm install
```

### 3️⃣ Configure Environment Variables
Create a `.env` file in the root directory and add:
```env
MONGO_URI=your-mongodb-connection-string
JWT_SECRET=your-jwt-secret
RAZORPAY_KEY_ID=your-razorpay-key-id
RAZORPAY_KEY_SECRET=your-razorpay-key-secret
EMAIL_USER=your-email@example.com
EMAIL_PASS=your-email-password
```

### 4️⃣ Start the Server
```sh
npm start
```

---

## 📡 Deployment

For production deployment:
1. Use **Docker** or **PM2** for process management.
2. Deploy on **AWS, DigitalOcean, or Heroku**.
3. Use **MongoDB Atlas** for cloud-based database management.

---

## 🔗 Repository Links

- **Frontend Repository**: [FuelOne Gas Slot Booking Frontend](https://github.com/Lekkaiyaraja/Gas-Slot-Booking-App-Frontend)
- **Backend Repository**: [FuelOne Gas Slot Booking Backend](https://github.com/Lekkaiyaraja/Gas-Slot-Booking-App-Backend)

---

## 📞 Contact

For inquiries or issues, feel free to reach out:

📧 **Email**: lekkaiyarajaraj2020@gmail.com  

🌐 **Website**: [Click Here](https://my-personal-portfolio-developer.netlify.app/)

🚀 **FuelOne - Powering Smart Refueling!**  

