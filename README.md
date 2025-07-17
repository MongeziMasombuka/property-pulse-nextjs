# 🏠 Property Pulse

**Property Pulse** is a full-featured real estate rental platform I built from the ground up using **Next.js**. It allows users to list, browse, and manage rental properties with rich features like messaging, image galleries, geolocation, social sharing, and more — all wrapped in a modern, responsive UI.

This project demonstrates advanced use of the **Next.js App Router**, **Server Actions**, **NextAuth**, **MongoDB**, **Cloudinary**, and other cutting-edge tools. It was designed as a production-grade full-stack application with performance, security, and user experience in mind.

---

## 🚀 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Environment Setup](#environment-setup)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

---

## 🌟 Features

- ✅ Google OAuth 2.0 authentication with session management
- 🏘 Full CRUD for property listings with multiple image uploads
- 💬 User-to-user messaging system with unread notifications
- 📸 Cloud image storage via Cloudinary and photo gallery viewer
- 🧭 Property search with filters, map markers, and saved listings
- 🔐 Secure, protected pages and route-based access control
- 📱 Responsive design using Tailwind CSS
- 🔔 Toast notifications, loading states, and elegant UI interactions

---

## 🧱 Tech Stack

| Layer           | Tools & Libraries                           |
| --------------- | ------------------------------------------- |
| Framework       | **Next.js 14** (App Router, Server Actions) |
| UI Styling      | **Tailwind CSS**, Headless UI               |
| Auth            | **NextAuth.js** (Google OAuth Provider)     |
| Backend         | MongoDB, Mongoose, Server Components        |
| Images          | Cloudinary, PhotoSwipe                      |
| UX Enhancements | React Icons, React Toastify, Spinners       |

---

## ⚙️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/property-pulse.git
   cd property-pulse
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Create `.env` file**

   Rename `.env.example` to `.env` and fill in your keys:

   ```env
   MONGODB_URI=your_mongodb_connection
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_secret
   NEXTAUTH_SECRET=a_random_secure_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_key
   CLOUDINARY_API_SECRET=your_cloudinary_secret
   NEXT_PUBLIC_MAPBOX_TOKEN=your_mapbox_token
   NEXT_PUBLIC_GOOGLE_GEOCODING_API_KEY=your_google_geocoding_api_key
   ```

---

## 🧪 Running Locally

Start the development server:

```bash
npm run dev
```

Visit: [http://localhost:3000](http://localhost:3000)

---

## 👨‍💻 Usage

As a user, you can:

- Register/login using your Google account
- Create, edit, and delete your own listings
- Browse listings by location, price, and type
- View listing details with gallery, and contact options
- Send private messages to owners
- Save favorite properties to your dashboard

As an admin (or the property owner), you can:

- Manage all your listings from your account
- View and respond to incoming messages

---

## 📁 Folder Structure

```
/app
  /(auth)           → Authentication routes (login, register)
  /dashboard        → User dashboard with protected routes
  /properties       → Property CRUD views
  /api              → Server actions & backend logic

/lib
  /cloudinary.ts    → Cloudinary config
  /auth.ts          → Auth utilities and NextAuth config

/components
  → UI elements (forms, cards, galleries, maps, etc.)
```

---

## 🙌 Acknowledgments

- Cloudinary for media hosting
- Google APIs for authentication
- [PhotoSwipe](https://photoswipe.com/) for image galleries

---

## ✅ TODO

- [ ] **Integrate Geolocation with Mapbox**  
      Display properties on an interactive map using `react-map-gl`.  
      Automatically set the map location based on user input or geocoded address.
- [ ] **Add Address Autocomplete & Reverse Geocoding (Google Maps API)**  
      Use the Google Places API for autocomplete in the property form.  
      Convert selected addresses into latitude/longitude coordinates.
- [ ] **Implement Stats & Engagement Tracking**  
      Track listing views, user logins, and message activity.  
      Display basic analytics in the user dashboard (e.g., total views, messages sent).
- [ ] **Deploy to Vercel**  
      Set up environment variables for production.  
      Connect to MongoDB Atlas and validate all production features.

---
