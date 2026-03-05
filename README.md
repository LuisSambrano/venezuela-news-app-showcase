<div align="center">

<!-- HEADER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,6,11&height=200&section=header&text=Libertad%20VZLA&fontSize=50&fontColor=fff&animation=twinkling&fontAlignY=35&desc=Full-Stack%20News%20Platform%20%7C%20Journalism%20%7C%20Open%20Source&descSize=18&descAlignY=55"/>

<!-- BADGES -->
<p>
  <img src="https://img.shields.io/badge/Type-Platform-blueviolet?style=for-the-badge" alt="Type: Platform"/>
  <img src="https://img.shields.io/badge/Next.js-16+-black?style=for-the-badge&logo=next.js" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Supabase-Database-green?style=for-the-badge&logo=supabase" alt="Supabase" />
  <img src="https://img.shields.io/badge/TailwindCSS-Styling-06B6D4?style=for-the-badge&logo=tailwindcss" alt="Tailwind CSS" />
</p>

<!-- LANGUAGE SWITCHER -->
<p>
  <a href="./README.md"><img src="https://img.shields.io/badge/🇺🇸_English-Selected-blue?style=flat-square" alt="English"/></a>
  <a href="./README.es.md"><img src="https://img.shields.io/badge/🇪🇸_Español-Available-lightgrey?style=flat-square" alt="Español"/></a>
  <a href="./README.pt.md"><img src="https://img.shields.io/badge/🇧🇷_Português-Available-lightgrey?style=flat-square" alt="Português"/></a>
</p>

</div>

---

**A high-performance journalism content management and news distribution system engineered with strict SSR, Server Actions, and a decoupled architecture.**

---

## 🏛️ Project Abstract

This repository contains the source code for a high-performance content management and news distribution system. Engineered with modern web standards, it leverages **Next.js Server-Side Rendering (SSR)**, **Server Actions**, and a **Supabase PostgreSQL** backend. The architecture is designed to prioritize fast content delivery, maintainability, and robust administrative workflows.

---

## ⚙️ Core Technical Features

### 1. Performance Engineering

Systematic optimization of network latency and rendering cycles. The platform adheres to Core Web Vitals targets utilizing React Server Components (RSC) and dynamic streaming to minimize Javascript bundles and improve Time to First Byte (TTFB).

### 2. Data Integrity & Security

Implemented with a decoupled architecture utilizing a granular identity validation layer. We leverage Supabase Row-Level Security (RLS) to enforce data access policies directly at the database layer, protecting administrative endpoints and editorial data.

### 3. Scalable Architecture

Follows a modular, component-based structure designed for high availability and separation of concerns. Strict typings and standardized React patterns ensure predictable maintenance cycles.

---

## 🏗️ Technical Architecture Overview

```text
venezuela-news-app/
├── src/
│   ├── app/                 # Next.js App Router & Server Components
│   │   ├── (cms)/           # Protected Administrative Layouts
│   │   ├── (marketing)/     # Public Access Routes (Landing & Feed)
│   │   └── actions/         # Next.js Server Actions (Backend Logic)
│   ├── components/          # Modular React Components (UI & Features)
│   ├── lib/                 # Core utilities, API clients & hooks
│   └── types/               # TypeScript Definitions & Interfaces
```

**Enterprise Tech Stack:**

- **Framework:** Next.js (App Router, Server Components)
- **Styling & UI:** Tailwind CSS, Framer Motion, Radix Primitives
- **Data Layer:** Supabase (PostgreSQL, Auth, Storage)
- **Engine:** TypeScript (Strict Mode)

---

## ⚙️ Installation & Development

Ensure you have `Node.js 18+` installed.

1. **Clone the repository:**

   ```bash
   git clone https://github.com/LuisSambrano/venezuela-news-app.git
   ```

2. **Install dependencies:**

   ```bash
   cd venezuela-news-app
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env.local` file in the root directory and add your Supabase keys:

   ```env
   NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
   ```

4. **Run the local development server:**
   ```bash
   npm run dev
   ```

---

## 🎨 Code Standards

This repository enforces strict engineering standards:

1. `npm run lint` must yield zero errors or warnings before committing.
2. `tsc --noEmit` must pass without type errors.
3. No `any` types allowed; use strict typing or `unknown` with Type Guards.
4. Conventional Commits are required for version control.

---

## 📄 License & Contributing

This project is proprietary. Please refer to `.agent/rules/PROTOCOL_ZERO.md` for internal architectural guidelines.

---

<div align="center">

_Architected by **Luis Sambrano**_

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,6,11&height=100&section=footer"/>

</div>
