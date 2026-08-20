# Re-Wire

**Live Demo:** [https://rewire-app1.vercel.app/](https://rewire-app1.vercel.app/)

## The Problem
E-waste is one of the fastest-growing waste streams globally, yet a massive 95% of it in India is handled by the unorganised, informal sector. This leads to severe environmental pollution, health hazards for informal workers, and a tremendous loss of valuable, recoverable raw materials like gold, copper, and rare earth elements. Furthermore, government regulations (E-Waste Rules 2022) mandate formal recycling targets, but authorized recyclers struggle to source steady, verifiable streams of e-waste directly from households.

## The Solution
Re-Wire bridges the gap between households generating e-waste and formal, CPCB-authorised recyclers. We provide a structured, verifiable, and rewarding supply chain pipeline. 

By using Re-Wire:
* **Households** are incentivised to dispose of their electronics responsibly through a transparent valuation engine and instant payouts.
* **Recyclers** get access to a consistent, sorted, and compliant stream of raw e-waste, helping them meet government-mandated EPR (Extended Producer Responsibility) quotas without relying on unpredictable informal channels.

## Key Features

### For Households (Users)
* **Real-time E-Waste Valuation:** Instantly estimate the reward value of items based on category and weight before scheduling a pickup.
* **Doorstep Scheduling:** Request convenient, free doorstep pickups tailored to specific localities.
* **Instant Wallet & Redemption:** Earn Re-Wire points upon successful collection. Redeem points directly for cash via UPI bank transfer or convert them into digital vouchers for popular brands like Amazon, Swiggy, and Flipkart.

### For Recyclers (Partners)
* **Partner Dashboard:** A dedicated interface to manage incoming requests, track monthly collection analytics, and monitor performance.
* **Verified Leads:** Access to pre-sorted, geo-located e-waste pickup requests from verified households.
* **EPR Compliance Tools:** Higher tier plans provide analytics and reporting to help formal businesses meet government quotas easily.

## Architecture & Tech Stack

This project is built as a unified monorepo containing both the frontend and backend.

* **Frontend:** React, Vite, React Router, Vanilla CSS, Stripe Elements
* **Backend:** Node.js, Express, MongoDB (Mongoose), JWT Authentication, Stripe SDK
* **Deployment:** Vercel (Serverless Functions)

## Local Development

### Prerequisites
* Node.js v18 or higher
* MongoDB connection string

### Setup

1. Clone the repository
2. Set up environment variables in the `rewire-backend` directory by creating a `.env` file with the following variables:
   ```
   PORT=5000
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   STRIPE_SECRET_KEY=your_stripe_secret_key
   ```
3. Install dependencies from the root directory:
   ```bash
   npm run install:all
   ```

4. Start the development servers:
   * Backend: Run `npm run dev` inside `rewire-backend`
   * Frontend: Run `npm run dev` inside `rewire-app`
