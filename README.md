# MERN Stack E-Commerce Website

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Introduction
This is a fully functional e-commerce website built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It provides users with a seamless online shopping experience, including product browsing, authentication, and payment processing.

## Features
- User authentication (JWT-based login & registration)
- Admin dashboard for product & order management
- Product listing, search, and filtering
- Shopping cart and checkout process
- Payment integration (e.g., Stripe/PayPal)
- Order tracking & management
- Responsive UI

## Tech Stack
- **Frontend:** React.js, Redux, Bootstrap/Tailwind CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JSON Web Tokens (JWT)
- **Payment Gateway:** Stripe/PayPal
- **Deployment:** Vercel/Netlify (Frontend), Heroku/Railway (Backend)

## Installation
### Prerequisites
Ensure you have the following installed:
- Node.js
- MongoDB
- npm or yarn

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. Install dependencies:
   ```sh
   cd backend
   npm install
   cd ../frontend
   npm install
   ```

3. Create a `.env` file in the backend directory and add:
   ```env
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_secret_key
   STRIPE_SECRET=your_stripe_key
   ```

4. Start the development servers:
   ```sh
   cd backend
   npm run dev
   cd ../frontend
   npm start
   ```

## Usage
- Visit `http://localhost:3000` to explore the frontend.
- Use `http://localhost:5000/api` for backend API endpoints.

## Folder Structure
```
├── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── config
│   ├── middleware
│   ├── server.js
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── redux
│   │   ├── App.js
│   │   ├── index.js
```

## API Endpoints
### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login

### Products
- `GET /api/products` - Fetch all products
- `GET /api/products/:id` - Fetch product by ID

### Orders
- `POST /api/orders` - Create a new order
- `GET /api/orders/:id` - Fetch order details

## License
This project is licensed under the MIT License.

