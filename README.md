# 🏡 HomeHaven – Full-Stack Travel Accommodation Platform

HomeHaven is a full-stack web application inspired by modern accommodation platforms, designed to provide a seamless experience for users to explore, review, and manage travel stays.

The platform supports both users and property owners, enabling listing management, booking interactions, and dynamic location visualization.

---

## 🌟 Key Features

* 🔐 **Authentication & Authorization**
  Secure user login/signup using Passport.js with session management.

* 🏠 **Property Listings (CRUD)**
  Owners can create, update, and delete listings with images and details.

* ✍️ **Reviews System (CRUD)**
  Users can add and delete reviews for listed properties.

* 🗺️ **Interactive Maps Integration**
  Location visualization using Mapbox for better user experience.

* ☁️ **Image Upload & Management**
  Integrated Cloudinary for storing and managing listing images.

* ✅ **Data Validation & Security**
  Server-side validation and schema enforcement for reliability.

* ⚠️ **Error Handling Middleware**
  Centralized error handling for improved backend stability.

---

## 🛠️ Tech Stack

### ⚙️ Backend

* Node.js
* Express.js
* MongoDB (Mongoose ODM)

### 🎨 Frontend

* EJS (Templating Engine)
* Bootstrap
* JavaScript

### 🔧 Tools & Services

* Passport.js (Authentication)
* Multer (File Uploads)
* Cloudinary (Cloud Storage)
* Mapbox (Maps Integration)

---

## 🏗️ Architecture

* MVC (Model–View–Controller) design pattern
* Modular and scalable backend structure
* RESTful routing and organized middleware usage

---

## 🚧 Project Status

* ✅ Core features fully implemented
* ✅ Backend tested and working in local environment
* ⚠️ Deployment in progress (currently resolving environment/configuration issues)

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/homehaven.git
```

### 2. Install dependencies

```bash
npm install
```

### 3. Setup environment variables

Create a `.env` file and configure:

```env
CLOUDINARY_KEY=your_key
CLOUDINARY_SECRET=your_secret
MAPBOX_TOKEN=your_token
SESSION_SECRET=your_secret
```

### 4. Run the application

```bash
npm start
```

---

## 🚀 Upcoming Enhancements

* 💳 Payment gateway integration
* ⭐ Ratings & advanced review system
* 🔎 Advanced search & filtering
* 🌐 Cloud deployment (Render / AWS / Vercel)

---

## 📸 Screenshots / Demo

*(Add UI screenshots or a demo video here)*

---

## 💡 Key Learnings

* Designed and implemented a full-stack system using MVC architecture
* Gained hands-on experience with authentication, sessions, and cookies
* Improved understanding of database relationships and schema design
* Learned real-world debugging and error handling techniques
* Built production-style backend with modular structure

---

## 🔗 Repository

GitHub: https://github.com/your-username/homehaven

---

## 🤝 Feedback

Feedback and suggestions are welcome! Feel free to open issues or contribute to the project.

---

## 📌 Note

This project reflects a practical implementation of real-world system design and backend development concepts. Deployment is currently in progress and will be available soon.
