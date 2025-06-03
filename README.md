# 🚀 Full-Stack Web Application – MERN, MEAN, Flask (with PWA Support)

A robust, full-featured **Full Stack Web Application** built using the **MERN**, **MEAN**, and **Flask** stacks. This project demonstrates the implementation of scalable, maintainable applications across **JavaScript** and **Python** ecosystems with features such as authentication, RESTful APIs, media uploads, and responsive UI. Additionally, this project has been enhanced to include **PWA (Progressive Web App)** capabilities for offline functionality and installability.

---

## 🔧 Tech Stack

### **Frontend:**
- **React.js** *(MERN)* / **Angular** *(MEAN)*  
- **State Management**: Context API / Redux *(MERN)* / **NgRx** *(MEAN)*  
- **Styling**: Tailwind CSS, **DaisyUI** (for pre-built UI components) / Bootstrap / CSS Modules  
- **Routing**: React Router *(MERN)* / Angular Router *(MEAN)*  
- **Build Tool**: **Vite** (Faster development and optimized production builds)

### **Backend:**
- **Node.js + Express.js** *(MERN & MEAN)*  
- **Flask (Python)** *(Flask Stack)*  
- **Real-Time Communication**: Socket.IO (for live updates, notifications, likes, and comments) *(Optional)*  

### **Database:**
- **MongoDB** (Mongoose ODM) *(MERN & MEAN)*  
- **SQLAlchemy + PostgreSQL / MySQL** *(Flask Stack)*

### **Authentication & Security:**
- **JWT (JSON Web Tokens)** for secure authentication  
- **bcrypt.js** for password hashing *(Node.js)*  
- **Werkzeug Security** *(Flask)*  
- **express-rate-limit** to prevent abuse (brute force, DoS attacks)  
- **helmet** to set secure HTTP headers  

### **Media Uploads:**
- **Multer** for handling file uploads *(Node.js)*  
- **Cloudinary** for media hosting (profile images, posts, etc.)

### **API Testing:**
- **Postman**  
- **Thunder Client** *(VS Code Extension)*

### **Environment Management:**
- **dotenv** for environment variable management  

### **Version Control:**
- **Git & GitHub**  

### **PWA (Progressive Web App) Integration:**
- **Service Worker** to enable offline functionality and faster loading times.
- **Web App Manifest**: Allows users to install the app on their devices.
- **Install Prompt**: Users can install the web app on their mobile or desktop for a native app experience.
  
---

## 🚀 Features

- **User Authentication & Authorization**: Login, registration, and secure access control with role-based authentication (Admin/User).  
- **CRUD Operations**: Complete Create, Read, Update, and Delete functionality for resources like posts, users, and more.  
- **Responsive UI**: Fully responsive UI built using Tailwind CSS, **DaisyUI**, or Bootstrap, ensuring a smooth experience on both desktop and mobile devices.  
- **Secure API Endpoints**: All endpoints are secured with JWT for protected routes and access control.  
- **Integrated Frontend and Backend**: Seamless integration between the frontend (React.js or Angular) and backend (Express.js or Flask), with proxy and CORS configuration.

---

## ✨ Key Features

- 🔐 **Secure Authentication**: Register, login, and securely authenticate users with JWT tokens.  
- 👤 **User Profiles**: Users can create and update their profiles, including uploading avatars and writing a bio.  
- 📝 **Create and Delete Tweets**: Users can post tweets, edit them, and delete them as needed.  
- ❤️ **Like & Comment on Tweets**: Real-time interactions such as liking and commenting on tweets, visible to all users in the app.  
- 👥 **Follow/Unfollow Users**: Build social connections by following or unfollowing other users, impacting the user’s personalized feed.  
- 📰 **Personalized Feed**: A dynamic, personalized feed of tweets from followed users, displaying the most recent content.  
- 🔍 **Search Functionality**: Easily search for users and tweets using keywords or hashtags.  
- 📷 **Profile Image and Post Media Uploads**: Users can upload images for their profile and share media in their posts, powered by Cloudinary for storage.  
- 🧾 **Responsive UI**: A mobile-first, responsive user interface designed for all screen sizes using Tailwind CSS and Bootstrap.  

---

## 🚀 Features Summary

- **User authentication & authorization** (Login/Register)  
- **Role-based access** (Admin/User)  
- **CRUD operations** with RESTful APIs  
- **Responsive design** for desktop and mobile  
- **Secure API endpoints** with JWT  
- **Rate limiting** using `express-rate-limit`  
- **Secure HTTP headers** with `helmet`  
- **Error handling** and **validations**  
- **Integrated frontend and backend** using proxy and CORS  
- **Fast Development** with **Vite** (for rapid build and hot reloading)  
- **Pre-built UI Components** from **DaisyUI** for fast prototyping  
- **PWA Features**:  
  - Service worker for offline capabilities
  - Ability to install the app as a native app on mobile and desktop.
  - Push notifications (optional)

---

## 💡 Additional Enhancements

- **Vite for Build Optimization**: Use Vite as a modern, lightning-fast alternative to Webpack, improving both development and production build times for your React/Angular frontend.
  
- **DaisyUI Components**: Easily integrate **DaisyUI**, a Tailwind CSS plugin, to leverage pre-designed components like cards, buttons, modals, and more, speeding up UI development.

- **Progressive Web App (PWA)**:  
  - Full offline functionality with a service worker.
  - Ability to install the app as a native app on mobile and desktop.
  - Seamless user experience with faster load times and automatic updates.

---

## 📁 Project Structure

```js
Aero Neura/
│
├── client/                      # React frontend
│   ├── public/                  # Static assets
│   └── src/
│       ├── components/          # Reusable UI components
│       ├── pages/               # Application pages (Feed, Profile, etc.)
│       ├── context/             # Global state (e.g., Auth, Feed)
│       ├── utils/               # Helper functions and constants
│       ├── App.js               # Main app component
│       └── index.js             # Entry point
│
├── server/                      # Node.js + Express backend
│   ├── config/                  # DB and cloud storage configuration
│   ├── controllers/             # Request handlers / controller logic
│   ├── models/                  # Mongoose schemas for MongoDB
│   ├── routes/                  # API routes
│   ├── middleware/              # Auth, error handling middleware
│   └── server.js                # Entry point for backend server
│
├── .env                         # Environment variables
├── package.json                 # Project dependencies and scripts
└── README.md                    # Project documentation
```

---

## 🛠️ Getting Started

### Prerequisites

- Node.js >= 14.x
- MongoDB (local or Atlas cloud DB)
- (Optional) Cloudinary for media storage

### 1. Clone the Repository

```bash
git clone https://github.com/aeroneura/aeroneura.github.io.git
cd aeroneura.github.io
```

### 2. Backend Setup

```bash
cd server
npm install
npm run dev
```

## Create a .env file in /server:

```shell
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

3. Frontend Setup


```bash
cd client
npm install
npm start
```

## 🌐 API Endpoints Overview

| Method | Route                   | Description                 |
| ------ | ----------------------- | --------------------------- |
| POST   | /api/auth/register      | Register a new user         |
| POST   | /api/auth/login         | Login and return JWT        |
| GET    | /api/users/\:id         | Get user profile            |
| PUT    | /api/users/\:id         | Update profile (avatar/bio) |
| POST   | /api/posts              | Create new tweet            |
| GET    | /api/posts/feed         | Get tweets from following   |
| POST   | /api/posts/\:id/like    | Like or unlike a tweet      |
| POST   | /api/posts/\:id/comment | Comment on a tweet          |