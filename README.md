# SuperShop

SuperShop is a full‑stack supermarket website built with a Node.js/Express backend and a React frontend. It supports user authentication, product management (including image uploads), secure payment processing with Stripe, and an infinite‑scroll product listing.

## Features

- **User Authentication**: Sign up, log in, and secure password storage with JWTs and bcryptjs.
- **Product Catalog**: CRUD operations for products, with image upload via Cloudinary.
- **Shopping Cart & Checkout**: Add/remove items, adjust quantities, and complete payment with Stripe.
- **Responsive UI**: Built with React, Tailwind CSS, and infinite scroll for smooth browsing.
- **Notifications & Alerts**: SweetAlert2 and react‑hot‑toast for user feedback.
- **API Documentation**: Full Postman collection included for easy API testing.

## Technology Stack

### Server

- **Express**
- **cors**
- **mongoose**
- **dotenv**
- **jsonwebtoken**
- **bcryptjs**
- **cookie-parser**
- **helmet**
- **multer**
- **Resend**
- **MongoDB Atlas**
- **Cloudinary**
- **Stripe (Server)**
- **nodemon**

### Client

- **Vite**
- **Tailwind CSS**
- **React**
- **react-router-dom**
- **react-icons**
- **axios**
- **react-redux**
- **sweetalert2**
- **react-hot-toast**
- **@tanstack/react-table**
- **react-infinite-scroll-component**
- **react-hook-form**
- **@stripe/stripe-js**

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/DanielWorking/SuperShop.git
   cd SuperShop
   ```

2. **Install dependencies**
   - **Server**
     ```bash
     cd server
     npm install
     ```
   - **Client**
     ```bash
     cd ../client
     npm install
     ```

3. **Create `.env` files**
   - **Server** (`server/.env`)
     ```bash
     FRONTEND_URL=
     MONGODB_URI=
     RESEND_API=
     SECRET_KEY_ACCESS_TOKEN=
     SECRET_KEY_REFRESH_TOKEN=
     CLOUDINARY_CLOUD_NAME=
     CLOUDINARY_API_KEY=
     CLOUDINARY_API_SECRET_KEY=
     STRIPE_SECRET_KEY=
     STRIPE_ENDPOINT_WEBHOOK_SECRET_KEY=
     ```
   - **Client** (`client/.env`)
     ```bash
     VITE_STRIPE_PUBLICATION_KEY=
     ```

## Running the App

- **Server**
  ```bash
  cd server
  npm run dev
  ```
- **Client**
  ```bash
  cd client
  npm run dev
  ```

Then open `http://localhost:5173` (or the port Vite reports) to view the app.

## Postman Documentation

Import the provided `[SuperShop.postman_collection.json](https://www.postman.com/spaceflight-geoscientist-34704202/workspace/supershop)` into Postman to explore all API endpoints, including authentication, product CRUD, and Stripe webhooks.

## Contributing

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a pull request

---

> **GitHub Repository:**
> https://github.com/DanielWorking/SuperShop
