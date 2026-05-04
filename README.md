# 🏡 HomeHaven – Full-Stack Travel Accommodation Platform

A full-stack Node.js/Express application for discovering and managing travel accommodations. Built using the MVC architecture, HomeHaven supports user authentication, CRUD operations for listings and reviews, image uploads via Cloudinary, interactive maps with Mapbox, and robust server-side validation.

---

## ⚡ Overview

**Tech Stack:** Node.js · Express · MongoDB (Mongoose) · EJS · Passport.js · Cloudinary · Mapbox

### Key Features:

* User authentication with sessions (Passport.js)
* CRUD operations for listings and reviews
* Image uploads and management using Cloudinary
* Interactive maps integration for location visualization
* Owner-based authorization (edit/delete control)
* Flash messages and centralized error handling
* Server-side validation for secure data handling

---

## 🧩 Project Structure (MVC)

* **Model:** `/models/` — Mongoose schemas (Users, Listings, Reviews)
* **View:** `/views/` — EJS templates and layouts
* **Controller:** `/controllers/` — Business logic and route handling

### Other Important Directories:

* `/routes/` — Express route definitions
* `/middleware/` — Authentication & authorization logic
* `/utils/` — Helpers (validation, Cloudinary config, error classes)
* `/public/` — Static assets (CSS, JS, images)
* `/init/` — Database seeding/setup scripts
* `app.js` — Main application entry point

---

## 🚀 Getting Started (Local)

### Prerequisites

* Node.js (v16+)
* npm 
* MongoDB (local or MongoDB Atlas)
* Cloudinary & Mapbox accounts (recommended)

---

## ⚙️ Installation

```bash
# Clone the repository
git clone: https://github.com/Anushka-0422/HomeHaven-Project.git

# Install dependencies
npm install
```

---

## 🔐 Environment Setup

Create a `.env` file in the root directory:

```env
MONGO_URI=mongodb://127.0.0.1:27017/homehaven
PORT=8080
SESSION_SECRET=your-secret-key

CLOUDINARY_CLOUD_NAME=your-cloud-name
CLOUDINARY_KEY=your-cloud-key
CLOUDINARY_SECRET=your-cloud-secret

MAPBOX_TOKEN=your-mapbox-token
```

---

## 🧠 Run the App

Start the server using nodemon:

nodemon app.js

App will run on:
👉 http://localhost:8080/listings

---

## 🗺️ Routes Summary

### Listings

| Method | Path               | Description          | Auth  |
| ------ | ------------------ | -------------------- | ----- |
| GET    | /listings          | View all listings    | No    |
| GET    | /listings/new      | Create listing form  | Yes   |
| POST   | /listings          | Add new listing      | Yes   |
| GET    | /listings/:id      | View listing details | No    |
| GET    | /listings/:id/edit | Edit listing form    | Owner |
| PUT    | /listings/:id      | Update listing       | Owner |
| DELETE | /listings/:id      | Delete listing       | Owner |

---

### Reviews

| Method | Path                            | Description   | Auth         |
| ------ | ------------------------------- | ------------- | ------------ |
| POST   | /listings/:id/reviews           | Add review    | Yes          |
| DELETE | /listings/:id/reviews/:reviewId | Delete review | Owner/Author |

---

### Users

| Method | Path      | Description   | Auth |
| ------ | --------- | ------------- | ---- |
| GET    | /register | Register form | No   |
| POST   | /register | Create user   | No   |
| GET    | /login    | Login form    | No   |
| POST   | /login    | Login user    | No   |
| GET    | /logout   | Logout user   | Yes  |

---

## 🚧 Project Status

* ✅ Core features implemented
* ✅ Fully functional in local environment
* ⚠️ Deployment in progress (environment/configuration issues being resolved)

---

## 🧰 Troubleshooting

| Issue                    | Fix                                        |
| ------------------------ | ------------------------------------------ |
| MongoDB connection error | Verify `MONGO_URI` and database status     |
| Cloudinary upload fails  | Check credentials in `.env`                |
| Map not loading          | Ensure valid `MAPBOX_TOKEN`                |
| Session issues           | Verify `SESSION_SECRET` and session config |

---

## 🤝 Contributing

* Fork the repository
* Create a new feature branch
* Commit and test your changes
* Submit a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👤 Author

**Anushka Bhosale**

For feedback or suggestions, feel free to open an issue or connect via GitHub.

---

## 📌 Note

HomeHaven is built as a production-style full-stack application focusing on real-world backend architecture, authentication, and scalable design. Deployment is currently in progress and will be available soon.

---

## ⚡ One more suggestion (startup-level polish)

Note: Ensure MongoDB service is running locally before starting the server.
