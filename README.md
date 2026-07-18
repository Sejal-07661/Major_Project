# 🏡 WanderStay

A full-stack Airbnb-style property listing and booking platform where users can list, browse, and review stays around the world.

**🔗 Live Demo:** [major-project-h9i3.onrender.com](https://major-project-h9i3.onrender.com)

> ⚠️ This app is hosted on a free Render instance, so it may take ~50 seconds to spin up on the first request after inactivity.

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Environment Variables](#environment-variables)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

## 📖 About

WanderStay is a full-stack web application inspired by Airbnb, built to practice and demonstrate core backend and full-stack concepts — authentication, authorization, RESTful routing, database modeling, and cloud media storage. Users can sign up, create property listings, leave reviews, and manage their own listings securely.

---

## ✨ Features

- 🔐 **User Authentication & Authorization** — Secure signup/login using Passport.js (local strategy), with session-based auth
- 🏠 **Listings CRUD** — Create, view, edit, and delete property listings
- ⭐ **Reviews** — Users can add and delete reviews on listings
- ☁️ **Cloud Image Uploads** — Listing images stored and served via Cloudinary
- 🗺️ **Map Integration** — Location display for listings
- 💬 **Flash Messages** — Real-time feedback for actions (success/error alerts)
- 🛡️ **Ownership Validation** — Only listing/review owners can edit or delete their content
- 🔄 **Method Override** — Clean RESTful routes using PUT/DELETE via forms
- ⚙️ **Centralized Error Handling** — Custom `ExpressError` class for consistent error responses

---

## 🛠️ Tech Stack

**Backend:** Node.js, Express.js
**Database:** MongoDB, Mongoose
**Templating:** EJS, EJS-Mate (layouts)
**Authentication:** Passport.js, Passport-Local
**Session Storage:** Express-Session, Connect-Mongo
**Media Storage:** Cloudinary
**Validation:** Joi (schema validation)
**Others:** Method-Override, Connect-Flash, dotenv

---

## 📁 Project Structure

Major_Project/
├── controllers/     # Route logic
├── init/            # DB seeding/initialization
├── models/          # Mongoose schemas (Listing, Review, User)
├── public/          # Static assets (CSS, JS)
├── routes/          # Express route definitions
├── utils/           # Helper utilities (ExpressError, wrapAsync)
├── views/           # EJS templates
├── app.js           # App entry point
├── cloudConfig.js   # Cloudinary configuration
├── middleware.js     # Auth & validation middleware
└── schema.js         # Joi validation schemas


---

## 🚀 Getting Started

### Prerequisites
- Node.js installed
- MongoDB Atlas account (or local MongoDB instance)
- Cloudinary account (for image uploads)

### Installation

```bash
git clone https://github.com/Sejal-07661/Major_Project.git
cd Major_Project
npm install
node app.js
```

The app will run on `http://localhost:3000` (or your configured port).

---

## 🔑 Environment Variables

Create a `.env` file in the root directory with the following:
ATLASDB_URL=your_mongodb_connection_string
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
SECRET=your_session_secret

---

## 🔮 Future Improvements

- Add search and filter functionality for listings
- Booking/reservation system with date availability
- Wishlist / favorites feature
- Rating system (star-based, currently CSS is in place)
- Payment gateway integration

---
