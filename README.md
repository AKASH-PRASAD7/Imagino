🖼️ Imagino – AI Image SaaS Platform

Imagino is a full-stack, AI-powered SaaS platform for intelligent image processing. With features like image restoration, recoloring, generative fill, object removal, and background removal, Imagino empowers users to effortlessly enhance and transform their images. It also provides a secure, credit-based monetization system and an engaging community showcase.

🧠 Features

🔐 Authentication & Authorization – Secure user registration and login using Clerk.

🌍 Community Showcase – Browse, search, and view image transformations with pagination.

🔎 Advanced Image Search – Find images based on their content.

🧽 Image Restoration – Repair old, blurry, or damaged photos using AI.

🎨 Image Recoloring – Intelligently replace colors of objects within an image.

🧠 Generative Fill – Fill in or replace parts of an image with AI-generated content.

❌ Object Removal – Remove unwanted elements or people with precision.

🧼 Background Removal – Isolate subjects by automatically removing the background.

💾 Downloadable Output – Save your transformed images in high quality.

ℹ️ Transformation Metadata – View details for each image, like transformation type, date, and user.

🧑‍💻 Profile Page – Track your image transformations and view your current credit balance.

💳 Stripe Integration – Securely purchase credits to use for image processing.

🎟️ Credits System – Each image transformation consumes credits, which can be earned or purchased.

📱 Responsive UI/UX – A seamless experience optimized for all screen sizes, from mobile to desktop.

🛠️ Tech Stack
Category Technology/Service
Frontend Next.js 14 (App Router), React, TypeScript
Backend Next.js API Routes
Database MongoDB
Auth Clerk
Payments Stripe
Media Cloudinary
UI/Styling Tailwind CSS, Shadcn/ui
📁 Folder Structure
Generated code
imagino/
├── app/ # Next.js App Router (pages and routes)
├── components/ # Reusable UI components
├── lib/ # Utility functions, helpers, and API definitions
├── models/ # Mongoose schemas for MongoDB
├── public/ # Static assets (images, icons, etc.)
├── styles/ # Global CSS styles
├── types/ # TypeScript type definitions
└── .env # Environment variables (not committed)

🔧 Environment Variables

Create a .env file in the root directory of the project and add the following variables:

Generated env

# NEXT.JS SERVER

NEXT_PUBLIC_SERVER_URL=http://localhost:3000

# MONGODB

MONGODB_URL=your_mongodb_connection_string

# CLERK AUTHENTICATION

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
WEBHOOK_SECRET=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# CLOUDINARY MEDIA STORAGE

NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

# STRIPE PAYMENTS

STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Env
IGNORE_WHEN_COPYING_END
🧪 Local Development

Follow these steps to get the project running on your local machine.

Clone the repository:

Generated bash
git clone https://github.com/your-username/imagino.git
cd imagino
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Bash
IGNORE_WHEN_COPYING_END

Install dependencies:

Generated bash
npm install
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Bash
IGNORE_WHEN_COPYING_END

Set up environment variables:
Create a .env file in the root and populate it with your keys as shown in the section above.

Run the development server:

Generated bash
npm run dev
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Bash
IGNORE_WHEN_COPYING_END

Open your browser and visit http://localhost:3000.

📸 Screenshots

Coming soon...

✨ Future Improvements

Transformation History: A detailed log of all user transformations with time-based filters.

Social Sharing: Allow users to share their creations directly to social media platforms.

Advanced Editing Tools: Implement layer controls, masking, and other manual editing features.

Subscription Tiers: Introduce monthly/yearly subscription plans alongside the credit system.

📄 License

This project is licensed under the MIT License. See the LICENSE file for more details.
