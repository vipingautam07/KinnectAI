# KinnectAI SaaS Platform

An advanced **AI-powered SaaS application** built with the **MERN stack**, integrating **Clerk authentication** and **subscription-based access**. This platform allows users to generate **articles, blog titles, images, edit images, and get document reviews** — with separate **Free** and **Premium plans**.

<p align="center">
  <img alt="Static Badge" src="https://img.shields.io/badge/Expess.js-gray?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/Node.js-darkgreen?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/React.js-blue?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/MongoDB-red?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/Tailwind%20CSS-purple?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/Gemini%20API-pink?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/Cloudinary%20API-blue?style=for-the-badge">
  <img alt="Static Badge" src="https://img.shields.io/badge/clerk-orange?style=for-the-badge">
</p>



## Features

- **Article & Blog Title Generation** (AI-powered content writing)  
- **AI Image Generation**  
- **Background Removal** (clean product photos, transparent backgrounds)  
- **Object Removal from Images** (seamless AI editing)  
- **Document Review** (AI-based feedback & improvements)  
- 🔑 **Clerk Authentication** (secure login & signup)  
- 💳 **Subscription-based Access**  
  - **Free Plan** → Access to **Title & Article Generation**  
  - **Premium Plan** → Unlocks **all features**  


## 🛠 Tech Stack

**Frontend**
- ⚛️ React (with Vite)
- 🎨 Tailwind CSS
- 🛣 React Router DOM
- 🔐 Clerk (authentication)
- 🔄 Axios (API calls)

**Backend**
- 🌐 Node.js + Express
- 🗄 MongoDB + Mongoose
- 🤖 AI Integrations (OpenAI, clipdrop)
- 🔑 JWT (for secure API communication)
- 💳 Payment Gateway (Stripe for subscriptions)


## 📂 Project Structure

```md
KinnectAI/
│
├── server/          # Express + MongoDB backend
│   ├── models/       # Mongoose schemas (User, Subscription, etc.)
│   ├── routes/       # API routes (AI tools, payments)
│   ├── middleware/   # Auth & subscription middleware
│   └── server.js
│
├── client/         # React + Vite frontend
│   ├── src/
│   │   ├── components/  # Navbar, FeatureCards, etc.
│   │   ├── context/     # Auth & Subscription context
│   │   ├── pages/       # Dashboard, Login, Pricing, etc.
│   │   └── App.jsx
│   └── index.html
│
└── README.md
```

---
## 🔧 Installation & Setup

### 1. Clone the repo
```bash
git clone https://github.com/
```

### 2. Backend setup
```bash
cd server
npm install
```

#### Create a .env file with:
- PORT=5000
- FRONTEND_URI = http://localhost:5173
- MONGO_URI=your_mongodb_connection
- GEMINI_API_KEY = your_gemini_api_key
- CLERK_SECRET_KEY=your_clerk_secret
- CLERK_PUBLISHABLE_KEY = your_clerk_public_key
- CLIPDROP_API_KEY = your_clipdrop_api_key
- CLOUDINARY_CLOUD_NAME = cloud_name
- CLOUDINARY_API_KEY =    cloudinary_api_key
- CLOUDINARY_API_SECRET = cloudinary_api_secret

### Start backend
```bash
npm run dev
```

### 3. Frontend setup
```bash
cd client
npm install
```

#### Create a .env file with:
- VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
- VITE_BASE_URL=http://localhost:5000

### Start frontend
```bash
npm run dev
```

### App will run at:
- Frontend → http://localhost:5173
- Backend  → http://localhost:5000

## 📜 License
This project is licensed under the [MIT License](./LICENSE).

