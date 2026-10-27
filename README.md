# ✨ السراج للعطور (Alsiraj Perfumes) – Luxury Fragrance E-Commerce Platform

[![Live Demo](https://img.shields.io/badge/Live_Demo-alsiraj--perfumes.com-D4AF37?style=for-the-badge&logo=google-chrome&logoColor=white)](https://alsiraj-perfumes.com/)
[![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-black?style=for-the-badge&logo=framer&logoColor=blue)](https://www.framer.com/motion/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Cloudinary](https://img.shields.io/badge/Cloudinary-Media-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)](https://cloudinary.com/)
[![SEO](https://img.shields.io/badge/SEO-JSON--LD_Structured_Data-0070F3?style=for-the-badge&logo=google&logoColor=white)](https://schema.org/)

> **A high-end, bespoke e-commerce boutique crafted for luxury oriental fragrances, French perfumes, pure oud, and authentic incense.** Built with Next.js 15, React 19, TypeScript, and MongoDB, engineered with a cinematic golden dark-mode aesthetic, interactive sliding cart drawer, olfactory notes pyramid breakdown, instant fuzzy search modal, and SEO-optimized JSON-LD schema markup.

---

## 📸 Preview

![Alsiraj Perfumes Preview](preview.png)

---

## 🌟 Key Features

- **💎 Luxury Aesthetic & Gold-Themed UI:** Custom royal gold & obsidian dark palette designed to reflect exclusivity, opulence, and craftsmanship with buttery-smooth **Framer Motion** micro-interactions.
- **👃 Olfactory Pyramids & Detailed Profiles:** Comprehensive breakdown for every perfume displaying Top Notes, Heart Notes, and Base Notes (النوتات العليا، قلب العطر، وقاعدة العطر) alongside bottle size selectors (50ml / 100ml) and longevity indicators.
- **🛒 Sliding Off-Canvas Cart Drawer (`CartDrawer.tsx`):** Seamless client-side shopping bag with real-time price recalculation, item quantity controls, cookie/local persistence, and WhatsApp order handoff.
- **🔍 Instant Modal Search (`SearchModal.tsx`):** Blazing-fast keyboard-accessible modal search with instant fuzzy query matching across perfume titles, olfactory families, and aromatic notes.
- **🏷️ Dynamic Fragrance Categorization:** Effortless multi-category filtering for Men, Women, Unisex, Oriental Luxury, Pure Musk, and Bukhoor (`CategoryBar.tsx`).
- **☁️ Cloudinary Media Optimization:** High-definition perfume bottle photography delivered with automated WebP format compression and global edge CDN caching for near-zero load times.
- **📈 Advanced SEO & JSON-LD Structured Data:** Integrated Schema.org product schemas (`JsonLd.tsx`) empowering search engines with rich product snippets, ratings, and price availability.
- **📱 Responsive & Touch-First Design:** Mobile-first responsive layout with intuitive navigation gestures, sticky headers, and smooth viewport adaptability.

---

## 🛠️ Tech Stack & Architecture

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Framework** | [Next.js 15 (App Router)](https://nextjs.org/) | Server-Side Rendering (SSR), Server Components & API routes |
| **Frontend Library** | [React 19](https://react.dev/) | Concurrent UI rendering & modern component lifecycle hooks |
| **Language** | [TypeScript 5](https://www.typescriptlang.org/) | Strict static type definitions across products and state |
| **Styling** | [Tailwind CSS](https://tailwindcss.com/) & CSS Modules | Bespoke luxury gold themes & modular component styles |
| **Animations** | [Framer Motion](https://www.framer.com/motion/) | Smooth slider transitions, hover dynamics & entry animations |
| **Database & ODM** | [MongoDB](https://www.mongodb.com/) & [Mongoose 9](https://mongoosejs.com/) | Persistent catalog database, user profiles & product schemas |
| **Media Delivery** | [Cloudinary](https://cloudinary.com/) | Cloud storage, responsive media optimization & CDN delivery |
| **State & Persistence** | React Context API & [js-cookie](https://github.com/js-cookie/js-cookie) | Cart drawer state, user session management & local storage |
| **Icons & UI** | [Lucide React](https://lucide.dev/) | High-precision visual iconography |

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v18.18.0 or newer)
- **MongoDB** instance (Local or Atlas)
- **Cloudinary** account credentials
- **npm**, **yarn**, or **pnpm**

### Environment Configuration

Create a `.env.local` file in the root directory:

```env
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/alsiraj
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
JWT_SECRET=your_secure_jwt_secret
NEXT_PUBLIC_SITE_URL=https://alsiraj-perfumes.com
```

### Installation & Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Ploger1979/alsiraj-perfumes-shop.git
   cd alsiraj-perfumes-shop
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start local development server:**
   ```bash
   npm run dev
   ```

4. **Open in browser:**
   Navigate to [http://localhost:3000](http://localhost:3000) to explore the boutique.

---

## 📦 Project Directory Structure

```plaintext
alsiraj-perfumes-shop/
├── app/                  # Next.js App Router (Pages, dynamic product routes & APIs)
├── components/           # Reusable luxury UI components
│   ├── CartDrawer.tsx    # Off-canvas sliding cart drawer
│   ├── SearchModal.tsx   # Interactive fuzzy search modal
│   ├── HeroSlider.tsx    # Animated luxury fragrance carousel
│   ├── ProductDetails.tsx# Fragrance pyramid notes & sizing breakdown
│   ├── CategoryBar.tsx   # Fragrance families & category bar
│   ├── Navbar.tsx        # Responsive luxury navigation header
│   ├── Footer.tsx        # Brand footer & social channels
│   └── JsonLd.tsx        # Schema.org structured data injection
├── context/              # CartContext & theme state providers
├── data/                 # Curated fragrance catalog & fragrance notes
├── lib/                  # MongoDB client connection & auth utilities
├── models/               # Mongoose schemas (Product.ts, User.ts)
├── public/               # Static assets, branding & preview media
├── preview.png           # Showcase hero preview image
├── next.config.ts        # Next.js configuration & image optimization domains
└── tsconfig.json         # TypeScript compiler configuration
```

---

## 👨‍💻 Author

**Ayman Plöger**  
- Portfolio: [aymanbyte-portfolio.netlify.app](https://aymanbyte-portfolio.netlify.app/)  
- GitHub: [@Ploger1979](https://github.com/Ploger1979)  
- LinkedIn: [Ayman Plöger](https://www.linkedin.com/in/ayman-pl%C3%B6ger/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).