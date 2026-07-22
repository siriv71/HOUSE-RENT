# 🏠 House Rent Management System (MERN Stack)

A **modern, responsive, and production-ready House Rent Management System** built using the **MERN Stack (MongoDB, Express.js, React.js, Node.js)**. The application enables users to browse rental properties, post listings, manage bookings, and provides an administrative dashboard for managing users, properties, and bookings.

---

# 📌 Features

## User Features

* User Registration
* User Login
* JWT Authentication
* Secure Password Hashing using bcryptjs
* Browse Rental Properties
* Advanced Property Search & Filters
* View Property Details
* Book Property
* Cancel Booking
* Booking History
* Add New Property
* Edit Property
* Delete Property
* User Dashboard
* Profile Management
* Responsive UI
* Image Upload Support

---

## Admin Features

* Admin Login
* Dashboard Analytics
* Manage Users
* Approve/Reject Property Listings
* Edit/Delete Properties
* Manage Bookings
* View Statistics
* Revenue & Booking Charts

---

# 🚀 Technology Stack

## Frontend

* React.js
* React Router
* Axios
* Bootstrap 5
* React Icons
* React Toastify
* Chart.js
* React ChartJS 2

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* bcryptjs
* dotenv
* Multer
* Express Validator
* CORS

---

# 📂 Project Structure

```
House-Rent-Management-System/
│
├── client/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       ├── pages/
│       ├── layouts/
│       ├── routes/
│       ├── services/
│       ├── context/
│       ├── hooks/
│       ├── utils/
│       ├── App.js
│       └── index.js
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── uploads/
│   ├── utils/
│   ├── seed/
│   ├── app.js
│   └── server.js
│
├── .env.example
├── package.json
└── README.md
```

---

# 🗄 Database Collections

## Users

| Field        | Type       |
| ------------ | ---------- |
| name         | String     |
| email        | String     |
| password     | String     |
| role         | User/Admin |
| phone        | String     |
| profileImage | String     |
| createdAt    | Date       |

---

## Properties

| Field          | Type     |
| -------------- | -------- |
| title          | String   |
| description    | String   |
| location       | String   |
| city           | String   |
| state          | String   |
| price          | Number   |
| propertyType   | String   |
| bedrooms       | Number   |
| bathrooms      | Number   |
| area           | Number   |
| images         | Array    |
| amenities      | Array    |
| owner          | ObjectId |
| approvalStatus | String   |
| availability   | Boolean  |
| createdAt      | Date     |

---

## Bookings

| Field         | Type                       |
| ------------- | -------------------------- |
| user          | ObjectId                   |
| property      | ObjectId                   |
| bookingDate   | Date                       |
| status        | Pending/Approved/Cancelled |
| paymentStatus | Pending/Paid               |
| createdAt     | Date                       |

---

# 🔐 Authentication

* JWT Authentication
* Protected Routes
* Role-Based Authorization
* Password Encryption (bcryptjs)
* Secure Environment Variables

---

# 📡 REST API

## Authentication

```
POST   /api/auth/register
POST   /api/auth/login
```

---

## Users

```
GET    /api/users/profile
PUT    /api/users/profile
```

---

## Properties

```
GET    /api/properties
GET    /api/properties/:id
POST   /api/properties
PUT    /api/properties/:id
DELETE /api/properties/:id
```

---

## Bookings

```
POST   /api/bookings
GET    /api/bookings
PUT    /api/bookings/:id
DELETE /api/bookings/:id
```

---

## Admin

```
GET    /api/admin/dashboard
GET    /api/admin/users
PUT    /api/admin/property/approve/:id
DELETE /api/admin/property/:id
```

---

# 🎨 User Interface

The application includes:

* Responsive Navigation Bar
* Hero Banner
* Featured Properties
* Property Cards
* Property Carousel
* Grid & List Views
* Search Filters
* User Dashboard
* Admin Dashboard
* Charts & Analytics
* Data Tables
* Toast Notifications
* Loading Spinners
* Modal Dialogs
* Responsive Footer

---

# 🔎 Advanced Search

Users can search by:

* Location
* Property Type
* Rent Range
* Bedrooms
* Furnishing
* Availability

---

# 📷 Property Features

Each property includes:

* Multiple Images
* Description
* Amenities
* Address
* Google Map Location
* Owner Information
* Rent Price
* Availability Status
* Contact Button
* Book Property Button

---

# 📈 Admin Dashboard

Dashboard Cards:

* Total Users
* Total Properties
* Total Bookings
* Pending Listings

Charts:

* Monthly Listings
* Booking Statistics
* Revenue Analytics

---

# ✅ Validation

The application validates:

* Required Fields
* Email Format
* Password Strength
* Phone Number
* Rent Price
* Property Images
* Booking Details

---

# ⚡ Performance Optimization

* MongoDB Query Optimization
* Pagination
* Lazy Loading Images
* Reusable React Components
* Code Splitting
* Error Boundaries
* Optimized API Responses

---

# 🔒 Security Features

* JWT Authentication
* Password Hashing
* Input Validation
* Protected APIs
* Role-Based Authorization
* Environment Variables
* CORS Configuration
* Centralized Error Handling
* Rate Limiting

---

# 🛠 Installation Guide

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/house-rent-management-system.git
```

---

## 2. Navigate to the Project

```bash
cd house-rent-management-system
```

---

## 3. Install Backend Dependencies

```bash
cd server
npm install
```

---

## 4. Install Frontend Dependencies

```bash
cd ../client
npm install
```

---

## 5. Configure Environment Variables

Create a `.env` file inside the **server** folder.

Example:

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key

NODE_ENV=development

CLIENT_URL=http://localhost:3000
```

---

## 6. Start the Backend

```bash
cd server
npm run dev
```

---

## 7. Start the Frontend

```bash
cd client
npm start
```

---

## 8. Open the Application

```
http://localhost:3000
```

Backend API:

```
http://localhost:5000
```

---

# 🌐 Deployment

## Frontend

* Vercel

## Backend

* Render

## Database

* MongoDB Atlas

---

# 📦 Sample Seed Data

Run:

```bash
npm run seed
```

This command inserts:

* Sample Users
* Sample Properties
* Sample Bookings

---

# 📄 Environment Variables

```
PORT
MONGO_URI
JWT_SECRET
NODE_ENV
CLIENT_URL
```

---

# 📋 Future Enhancements

* Wishlist
* Online Payment Gateway
* Forgot Password (Email OTP)
* Google Maps Integration
* Real-Time Chat
* Property Reviews & Ratings
* Push Notifications
* Email Notifications
* Dark Mode
* Progressive Web App (PWA)

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# 📜 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

**Your Name**

* GitHub: https://github.com/your-username
* Email: [your-email@example.com](mailto:your-email@example.com)

---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub.
