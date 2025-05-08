# 🖼️ Background Remover Pro

**Visual Cleanup** is a full-stack image background removal application built with the **MERN stack**. It provides users with the ability to upload images and seamlessly remove their backgrounds using the **ClipDrop API**. The application features a **credit-based system powered by Razorpay**, where users purchase credits to remove images. It also integrates **Clerk** for secure authentication and user management.

---

## 📌 Project Overview

- **Users** can register and log in via **Clerk**.
- Users can **purchase credits** via **Razorpay** to remove image backgrounds.
- Each successful background removal deducts **one credit**.
- Images are processed through the **ClipDrop API** for clean, high-quality background removal.
- Users can download their processed images directly after successful removal.

---

## ✨ Features

### 🏠 Public Homepage Features

- **Hero Section with App Overview**
- **Login / Sign-Up via Clerk**
- **Pricing or Credit Purchase Section**
- Clean, modern UI for a simple and intuitive user experience.

---

### 👤 User Features

After securely logging in via **Clerk**, users can:

- **Purchase Credits**
  - Integrated **Razorpay payment gateway**.
  - Buy credits in predefined bundles.

- **Upload and Remove Image Backgrounds**
  - Upload images from local storage.
  - Use credits to process images via **ClipDrop API**.
  - Download the background-removed image instantly.

- **Credit Counter**
  - Real-time display of remaining credits.
  - Credits deducted **only after successful background removal**.

---

## 📊 API Integration

**ClipDrop API** is used to handle the background removal process:

- Sends image data via API call.
- Receives processed image with transparent background.
- Ensures high-quality, clean cuts around the subject.

---

## 🛠️ Tech Stack

| Technology        | Usage                          |
|:-----------------|:--------------------------------|
| React.js          | Frontend Development            |
| Node.js + Express.js | Backend APIs               |
| MongoDB           | Database                        |
| Clerk             | Authentication                  |
| Razorpay          | Payment Gateway Integration     |
| ClipDrop API      | Image Background Removal        |
| Vercel            | Frontend Deployment             |
| Render / Vercel   | Backend Deployment              |

---

## 🚀 Live Demo

🌐 [Check it out here](https://visual-cleanup-oqyn.vercel.app) — 

---

## Getting Started

To get started with the Visual Cleanup project, follow these steps:

1. Clone the repository from GitHub:

2. **Set Environment Variables**: Navigate to the `frontend` and `backend` folders and add necessary environment variables. You may need to create a `.env` file and configure it with required variables:
   In the backend/.env file:

   ```
   MONGODB_URI = your-mongo-url
   CLERK_WEBHOOK_SECRET=your-clerk-webhook-secret
   CLIPDROP_API=your-clipdrop-api-key
   RAZORPAY_KEY_ID=your-razorpay-key-id
   RAZORPAY_KEY_SECRET=your-razorpay-key-secret
   CURRENCY = 'INR'
   ```

   In the frontend/.env file:

   ```
   VITE_CLERK_PUBLISHABLE_KEY = your-publishable-key 
   VITE_BACKEND_URL = your-server-url
   VITE_RAZORPAY_KEY_ID = your-razorpay-key-id
   ```

3. **Install Dependencies**: Install dependencies in the `frontend` and `backend` folders using npm or yarn:

   ```
   cd frontend
   npm install
   cd ../backend
   npm install
   ```

4. **Start the Backend Server**: In the `backend` folder, start the development server using npm:

   ```
   npm run server
   ```

5. **Start the Frontend**: In the `frontend` folder, start the frontend application:

   ```
   npm run dev
   ```
