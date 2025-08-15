# 🚢 Smart Freight & Storage Planner

![Next.js](https://img.shields.io/badge/Next.js-15.4.6-black)
![Prisma](https://img.shields.io/badge/Prisma-ORM-blue)
![Neon](https://img.shields.io/badge/Postgres-Neon-green)
![Gemini API](https://img.shields.io/badge/AI-Gemini-orange)
![TailwindCSS](https://img.shields.io/badge/Style-TailwindCSS-blueviolet)

A logistics management platform to handle **shipments**, **voyages**, **AI-assisted planning**, and **tracking**. Built with **Next.js App Router**, **Prisma ORM**, **Neon Postgres**, and **Google Gemini API**, styled with **TailwindCSS** and deployed on **Vercel**.

<div align="center">
 <img src="https://via.placeholder.com/800x400?text=Smart+Freight+%26+Storage+Planner" alt="Smart Freight & Storage Planner Screenshot">
</div>

---

## 🌐 Live Demo

Try it online:  
[🔗 Live Web App](https://your-vercel-app-link.vercel.app/)

---

## ✨ Features

- **Shipments CRUD** – Manage shipments with weight, volume, status, and priority  
- **Voyages CRUD** – Create voyages with capacity, dates, and lanes  
- **Tracking Events** – Log shipment events with location & time  
- **Auto-Assign** – Rule-based assignment of shipments to voyages  
- **AI Auto-Assign** – Gemini-powered smart assignment with capacity & route awareness  
- **AI Console** – Ask natural language questions grounded in DB data  
- **ETA+ Predictions** – Mock delay prediction tool  
- **Snapshot Caching** – Avoids heavy DB scans for AI context

---

## 🎥 Live Demo & Walkthrough

[![Watch the demo](https://img.youtube.com/vi/VIDEO_ID_HERE/0.jpg)](https://your-demo-video-link)

<p align="center"><i>Click the image above to watch a quick demo of the Smart Freight & Storage Planner</i></p>

---

## 📋 Prerequisites

- Node.js 18+
- Neon Postgres account ([Get started here](https://neon.tech))
- Gemini API Key ([Get it here](https://ai.google.dev/gemini-api/docs/api-key))
- Vercel account for deployment

---

## 🔧 Installation (Local)

```bash
git clone https://github.com/your-username/shipsy-assignment.git
cd shipsy-assignment
npm install

Create .env with:

DATABASE_URL="your-neon-pooled-url"
DIRECT_URL="your-neon-direct-url"
JWT_SECRET="your-secret"
GEMINI_API_KEY="your-gemini-key"


Run migrations:

npx prisma generate
npx prisma migrate dev --name init


Start dev server:

npm run dev

🛠 How It Works

Rule-based auto-assign: Matches shipments to voyages based on lane, date, capacity, and priority

AI-assisted planning: Gemini selects optimal assignment plan and explains decisions

AI Console: Queries the DB through structured tools with natural language

Snapshot caching: Reduces token usage by summarizing shipments and voyages for the LLM

📦 Tech Stack

Next.js (Full-stack React Framework)

Prisma ORM + Neon Postgres

Google Gemini API (LLM)

TailwindCSS (Styling)

JWT (Authentication)

Vercel (Deployment)

☁️ Deployment (Vercel)

Push your project to GitHub

Import it to Vercel

Add environment variables from .env to Vercel dashboard (Production scope)

Vercel will run:

postinstall: prisma generate
vercel-build: prisma generate && next build


Assign a custom domain & update DNS records if needed

🔐 API Key Setup

Get your Gemini API key from Google Gemini Studio

Set it in .env:

GEMINI_API_KEY=your_key

👤 Author

Your Name
GitHub: @your-username
Project: Smart Freight & Storage Planner

📄 License

This project is licensed under the MIT License — see the LICENSE file.

⭐️ Support

If you found this project helpful, consider giving it a ⭐️ on GitHub!
