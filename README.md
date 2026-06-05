# ✍️ WriteFlow AI - AI-Powered Content Creation Platform

<div align="center">

**The all-in-one AI workspace for content creators, marketers, and businesses to generate, rewrite, and optimize content 10x faster**

[![Next.js](https://img.shields.io/badge/Next.js-14.2-000000?style=flat&logo=next.js&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat&logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-3.4-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![AI SDK](https://img.shields.io/badge/Vercel_AI_SDK-6.0-000000?style=flat&logo=vercel&logoColor=white)](https://sdk.vercel.ai/)
[![Prisma](https://img.shields.io/badge/Prisma-5.22-2D3748?style=flat&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#-license--contributions)

<div align="center">
  <a href="https://write-flow-ai-tau.vercel.app" target="_blank">
    <img
      src="https://img.shields.io/badge/WRITEFLOW_AI-LIVE%20DEMO-7c3aed?style=for-the-badge&logo=vercel&logoColor=white&labelColor=111827"
      alt="WRITEFLOW AI Live Demo"
    />
  </a>
</div>

</div>

---

## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#️-tech-stack)
- [Software Architecture](#️-software-architecture)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Database Schema](#-database-schema)
- [AI Agent System](#-ai-agent-system)
- [License & Contributions](#-license--contributions)

---

## 🎯 About The Project

**WriteFlow AI** is a comprehensive AI-powered content creation platform that transforms how professionals create, refine, and manage content. Built on Next.js 14 with the Vercel AI SDK and powered by Groq's lightning-fast LLM infrastructure, WriteFlow delivers enterprise-grade content generation with sub-second response times.

### Why WriteFlow AI?

- **Intelligent AI Agents**: Purpose-built agents for drafting, rewriting, and chat assistance with context-aware responses
- **Lightning-Fast Generation**: Groq-powered inference delivers complete blog posts in seconds
- **Complete Content Lifecycle**: From initial draft through refinement to export-ready copy
- **Advanced Analytics**: Track AI usage and user performance metrics

---

## ✨ Key Features

### 🤖 AI Agent Ecosystem

- **✍️ Draft Agent**: Generate long-form blog posts, landing pages, and articles from minimal prompts.
- **🔄 Rewrite Agent**: Transform existing text with tone modulation and structural enhancements.
- **💬 Chat Assistant**: Contextual Q&A for content strategy, SEO tips, and writing guidance.

### 🏢 Dashboards and Analytics
- Personal content generation history with full-text search.
- Saved drafts and works-in-progress.
- Usage analytics tracking AI token limits.

### 🔍 Content Management
- **Document Library**: Organize generated content seamlessly.
- **Version History**: Keep track of templates and usage logs.

---

## 🛠️ Tech Stack

WriteFlow AI is built as a monolithic Next.js application that handles both frontend presentation and backend API logic, connecting directly to a PostgreSQL database and AI inference APIs.

- **[Next.js 14.2](https://nextjs.org/)** — React framework with App Router, API routes, server components, and streaming
- **[React 18](https://react.dev/)** — Concurrent rendering, Suspense
- **[TypeScript 5](https://www.typescriptlang.org/)** — Type safety across components and APIs
- **[Tailwind CSS 3.4](https://tailwindcss.com/)** — Utility-first styling with Shadcn UI components
- **[Vercel AI SDK 6.0](https://sdk.vercel.ai/)** — Unified AI abstraction with streaming support
- **[NextAuth.js](https://next-auth.js.org/)** — Authentication ecosystem
- **[Prisma](https://www.prisma.io/)** — Next-generation Node.js and TypeScript ORM for connecting to PostgreSQL
- **[Groq SDK](https://groq.com/)** — Fast LLM inference API (`llama-3.3-70b-versatile` integration)
- **[Stripe](https://stripe.com/)** — Billing and subscriptions integration

> **Note**: This repository also contains an experimental `writeflow-ai-backend` directory based on Express and MongoDB. The primary application, however, operates fully via the `writeflow-ai-frontend` Next.js full-stack framework.

---

## 🏗️ Software Architecture

WriteFlow AI utilizes Next.js API routes for secure backend functionality, interacting directly with Prisma (PostgreSQL) for state management, NextAuth for sessions, and Groq for LLM completion streams.

```mermaid
graph TD
    Client[User Browser]
    
    subgraph Frontend [writeflow-ai-frontend (Next.js Monolith)]
        NextJS[Next.js App Router]
        APIHandler[Next.js API Routes]
        AIAgent[Vercel AI SDK]
        PrismaORM[Prisma ORM]
    end
    
    Client -->|HTTPS Request| NextJS
    NextJS -->|Internal API Call| APIHandler
    NextJS -->|AI Stream Hook| AIAgent
    
    APIHandler -->|Database Query| PrismaORM
    AIAgent -->|Stream Request| APIHandler
    
    APIHandler -->|Auth Verification| NextJS
    APIHandler -->|LLM Request| GroqAPI[Groq API]
    
    PrismaORM -->|SQL Queries| DB[(PostgreSQL)]
    
    GroqAPI -->|Token Stream| APIHandler
    APIHandler -->|Token Stream| AIAgent
    AIAgent -->|React Stream| Client
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v18.0.0 or higher)
- **npm** (v9.0.0 or higher)
- A **Groq account** with API key (for AI inference)
- Access to a **PostgreSQL** database (e.g., local, Supabase, Neon)

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/SiratimMChy/Writeflow-AI.git
cd Writeflow-AI/writeflow-ai-frontend
```

2. **Install Dependencies**

```bash
npm install
```

3. **Configure Environment Variables**

Create a `.env` file based on `.env.example` and configure your variables (Database URL, NextAuth secrets, Groq API key, etc.):
```bash
cp .env.example .env
```

4. **Initialize the Database**

```bash
npx prisma generate
npx prisma db push
```

5. **Start the Development Server**

```bash
npm run dev
```

Navigate to `http://localhost:3000` to view the application.

---

## 📖 Usage

1. **Create an Account**: Navigate to `/register` and provide your details to access the AI generation capabilities.
2. **Generate Content**: Navigate to **Draft Agent**. Enter a prompt (e.g., "Write a blog post about sustainable fashion") and watch the AI stream the content.
3. **Refine Output**: Use the **Rewrite Agent** to transform text tones or adjust lengths.
4. **Organize Documents**: Save and categorize your generated outputs in the Documents library.
5. **Monitor Usage**: Check your Analytics page to ensure you stay within your AI token limits.

---

## 📁 Project Structure

```
writeflow-ai/
├── writeflow-ai-frontend/       # The primary Next.js Full-Stack Application
│   ├── public/                  # Static assets
│   ├── src/                     # Source code
│   │   ├── app/                 # Next.js App Router (Pages & API Routes)
│   │   ├── components/          # Reusable React UI components (Shadcn UI)
│   │   ├── lib/                 # Utility functions, Prisma Client, Groq config
│   │   └── types/               # TypeScript definitions
│   ├── prisma/                  # Prisma schema models (schema.prisma)
│   ├── package.json             # Application dependencies
│   └── tailwind.config.ts       # Styling configuration
│
├── writeflow-ai-backend/        # Deprecated/Experimental Express Backend
│   ├── src/                     # Source code
│   │   ├── config/              # Configuration files
│   │   ├── middlewares/         # Express middlewares
│   │   ├── modules/             # API modules (controllers, routes, services)
│   │   └── server.ts            # Entry point
│   ├── package.json             # Backend dependencies
│   └── tsconfig.json            # TypeScript configuration
│
└── README.md                    # This file
```

---

## 💾 Database Schema

The core Next.js application relies on Prisma to manage a PostgreSQL database. Key models include:

- **User / Account / Session**: Managed by NextAuth for authentication. Contains user roles, subscription plans, and Stripe IDs.
- **Document**: Stores all generated content, categorizing them by draft, rewrite, or blog states.
- **Template**: Houses predefined frameworks and their respective prompts for consistent AI outputs.
- **AIUsageLog**: Tracks token utilization and agent interactions for every user to enforce tier limits.

---

## 🤖 AI Agent System

WriteFlow AI implements its intelligent logic directly within Next.js API Routes (`/api/ai/...`) using the `groq-sdk`:

1. **Authentication Gate**: Every request verifies the active session.
2. **Rate Limiting Checks**: Queries the `AIUsageLog` via Prisma to ensure the user has sufficient usage limits (e.g., Free vs. Premium tiers).
3. **Stream Resolution**: Utilizes `llama-3.3-70b-versatile` via Groq's chat completions to return a readable stream directly to the client's Vercel AI SDK hooks (`useChat` / `useCompletion`).

---

## 📄 License & Contributions

This project is open-source and distributed under the **MIT License**.

We welcome contributions! Please feel free to open a Pull Request or issue if you find any bugs or have feature requests.

<div align="center">

**Maintained by Siratim Mustakim Chowdhury**

[![GitHub](https://img.shields.io/badge/GitHub-SiratimMChy-181717?style=flat&logo=github)](https://github.com/SiratimMChy)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Siratim%20Mustakim-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/siratim-mustakim-chowdhury/)
[![Email](https://img.shields.io/badge/Email-chowdhurysiratimmustakim@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chowdhurysiratimmustakim@gmail.com)

</div>
