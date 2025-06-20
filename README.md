# 🖼️ Imagino - AI Image SaaS Platform

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?logo=mongodb&logoColor=white)](https://www.mongodb.com/)

> A full-stack, AI-powered SaaS platform for intelligent image processing and transformation.

Imagino empowers users to effortlessly enhance and transform their images with cutting-edge AI technology. From image restoration to generative fill, our platform provides professional-grade tools with a secure, credit-based monetization system and an engaging community showcase.

## ✨ Features

### Core Image Processing

- **🧽 Image Restoration** - Repair old, blurry, or damaged photos using advanced AI algorithms
- **🎨 Image Recoloring** - Intelligently replace colors of objects within images
- **🧠 Generative Fill** - Fill in or replace parts of images with AI-generated content
- **❌ Object Removal** - Remove unwanted elements or people with precision
- **🧼 Background Removal** - Automatically isolate subjects by removing backgrounds

### Platform Features

- **🔐 Secure Authentication** - User registration and login powered by Clerk
- **🌍 Community Showcase** - Browse, search, and view transformations with pagination
- **🔎 Advanced Image Search** - Find images based on their content
- **💾 High-Quality Downloads** - Save transformed images in premium quality
- **ℹ️ Transformation Metadata** - Detailed information for each transformation
- **🧑‍💻 Personal Profile** - Track transformations and monitor credit balance
- **💳 Secure Payments** - Credit purchasing through Stripe integration
- **🎟️ Credits System** - Flexible pay-per-use model for image processing
- **📱 Responsive Design** - Seamless experience across all devices

## 🛠️ Tech Stack

| Category           | Technology                                 |
| ------------------ | ------------------------------------------ |
| **Frontend**       | Next.js 14 (App Router), React, TypeScript |
| **Backend**        | Next.js API Routes                         |
| **Database**       | MongoDB                                    |
| **Authentication** | Clerk                                      |
| **Payments**       | Stripe                                     |
| **Media Storage**  | Cloudinary                                 |
| **UI/Styling**     | Tailwind CSS, Shadcn/ui                    |

## 📁 Project Structure

```
imagino/
├── app/                    # Next.js App Router (pages and routes)
├── components/             # Reusable UI components
├── lib/                    # Utility functions, helpers, and API definitions
├── models/                 # Mongoose schemas for MongoDB
├── public/                 # Static assets (images, icons, etc.)
├── styles/                 # Global CSS styles
├── types/                  # TypeScript type definitions
└── .env                    # Environment variables (not committed)
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm
- MongoDB database
- Clerk account for authentication
- Cloudinary account for media storage
- Stripe account for payments

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/AKASH-PRASAD7/Imagino.git
   cd imagino
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:

   ```env
   # NEXT.JS SERVER
   NEXT_PUBLIC_SERVER_URL=http://localhost:3000

   # MONGODB
   MONGODB_URL=your_mongodb_connection_string

   # CLERK AUTHENTICATION
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   WEBHOOK_SECRET=your_webhook_secret
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

   # CLOUDINARY MEDIA STORAGE
   NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret

   # STRIPE PAYMENTS
   STRIPE_SECRET_KEY=your_stripe_secret_key
   STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
   NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
   ```

4. **Run the development server**

   ```bash
   npm run dev
   ```

5. **Open your browser**

   Navigate to [http://localhost:3000](http://localhost:3000) to see the application.

## 📊 Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server
npm run lint         # Run ESLint
npm run type-check   # Run TypeScript type checking
```

## 🔧 Configuration

### Database Setup

Ensure your MongoDB connection string is properly configured in the `.env` file. The application uses Mongoose for database operations.

### Authentication Setup

Configure Clerk authentication by:

1. Creating a Clerk application
2. Setting up your authentication providers
3. Configuring redirect URLs
4. Adding webhook endpoints for user synchronization

### Payment Setup

Set up Stripe for credit purchases:

1. Create a Stripe account
2. Configure webhook endpoints
3. Set up product pricing
4. Test payment flows in development mode

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
