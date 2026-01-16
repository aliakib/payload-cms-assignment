# Restroworks Assignment – CMS Driven Website

This project is built as part of the Restroworks Round 2 assignment.  
It demonstrates a **CMS-driven website** using **PayloadCMS** and **Next.js (App Router)** with real-world architecture, multilingual support, and deployment.

The focus of this assignment is **CMS modeling, frontend integration, and clean architecture**, not just UI.

---

## 🚀 Tech Stack

**Frontend**
- Next.js (App Router)
- TypeScript
- Tailwind CSS
- next/image

**Backend / CMS**
- PayloadCMS (Website Template)
- MongoDB Atlas

**Deployment**
- AWS EC2
- PM2 (process manager)

---

## 🧠 Architecture Overview

This project uses the **PayloadCMS website template**, where the CMS and frontend are bundled into a **single Node.js application**.

PayloadCMS manages all content and exposes APIs, while Next.js renders the frontend.




---

## 📄 Features Implemented

- CMS-driven Home page
- Hero, Features, Testimonials blocks
- Contact form with DB storage
- Multilingual content (English + Hindi)
- Responsive testimonial carousel
- SEO metadata from CMS
- CSS-only animations

---

## 🧩 CMS Modeling

### Pages Collection
- Slug-based pages
- SEO fields
- Block-based layout

### Custom Blocks
- **Hero** (localized title & subtitle)
- **Features** (title, description, image)
- **Testimonials** (image, name, role, rating, message)

Blocks are reusable and configurable from the Payload admin panel.

---

## 🌍 Multilingual Support

Multilingual content is handled using **PayloadCMS localization**.

- Supported locales: **English (en)** and **Hindi (hi)**
- Selected CMS fields are localized
- Language is selected from the frontend using a query parameter

Examples:
Frontend fetches localized content dynamically from the CMS.

---

## ⭐ Testimonials Carousel

- CSS scroll-snap based carousel
- Mobile: 1 card
- Tablet: 2 cards
- Desktop: 3 cards
- Desktop navigation arrows
- Star ratings
- No external carousel libraries

---

## 🖥️ Running the Project Locally (FULL STEPS)

### 1️⃣ Prerequisites

Make sure you have:
- Node.js (v18 or later)
- npm
- MongoDB (local or MongoDB Atlas)

---

### 2️⃣ Clone the Repository

### bash
git clone <repository-url>
cd <project-folder>

### 3️⃣ Install Dependencies
npm install

### 4️⃣ Environment Configuration
# Create a .env file in the project root:

NODE_ENV=development
PAYLOAD_SECRET=your-secret-key
MONGODB_URI=your-mongodb-connection-string
PAYLOAD_PUBLIC_SERVER_URL=http://localhost:3000

5️⃣ Run the Development Server
npm run dev

