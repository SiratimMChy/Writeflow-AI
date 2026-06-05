# ✍️ WriteFlowAi - AI-Powered Content Creation Platform

> Discover a seamless, lightning-fast workspace for generating, rewriting, and optimizing content powered by cutting-edge AI.

<div align="center">

[![Next.js](https://img.shields.io/badge/Next.js-14.2.15-000?style=flat&logo=next.js&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=flat&logo=react&logoColor=white)](https://react.dev/)
[![Prisma](https://img.shields.io/badge/Prisma-5.22.0-2D3748?style=flat&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16.x-4169E1?style=flat&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-3.4.1-06B6D4?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Groq AI](https://img.shields.io/badge/Groq%20AI-LLaMA%203.3-FF6B35?style=flat&logo=ai&logoColor=white)](https://groq.com/)

<div align="center">

<a href="https://write-flow-ai-tau.vercel.app" target="_blank" rel="noopener noreferrer">
  <img 
    src="https://img.shields.io/badge/WRITEFLOW-LIVE%20DEMO-7c3aed?style=flat&labelColor=000000"
    alt="WRITEFLOW AI Live Demo"
  />
</a>

</div>

</div>

---

## 📋 Table of Contents

- [About The Project](#about-the-project)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [API Documentation](#api-documentation)
- [Deployment](#deployment)
- [Security & Best Practices](#security--best-practices)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

---

## 🎯 About The Project

**WriteFlow AI** is a full-stack SaaS platform that revolutionizes how professionals, marketers, and content creators generate, refine, and manage their content. Powered by Groq's cutting-edge AI technology and built entirely on the Next.js App Router, WriteFlow combines intelligent templates with lightning-fast, real-time streaming interfaces.

### Core Value Proposition

- **AI-Powered Creation**: Groq's LLaMA 3.3 70B model provides highly intelligent, context-aware content generation instantly.
- **Secure Sessions & Payments**: Stripe integration ensures robust payment processing alongside NextAuth for role-based access.
- **Enterprise-Grade Database**: Prisma ORM mapped to PostgreSQL guarantees data consistency and type-safe schema modeling.
- **Mobile-First Design**: Fully responsive interface optimized for all devices with seamless dark mode support via Shadcn UI.
- **Scalable Architecture**: True serverless deployment ready on Vercel with streaming API endpoints.

### Why Choose WriteFlow AI?

Unlike traditional text generators, WriteFlow AI stands out by:
- Combining specialized AI Agents (Draft, Rewrite, Chat) under one unified workspace.
- Enforcing subscription tiers and precise AI token consumption limits securely.
- Offering comprehensive admin analytics for monitoring platform growth and user activity.
- Utilizing a unified monolithic React frontend architecture for an incredibly fast user experience.

---

## ✨ Key Features

### 🤖 AI-Powered Content Engine

- **Intelligent Draft Agent**: Generates long-form blog posts, landing pages, and articles from minimal prompts in seconds.
- **Rewrite & Optimization Agent**: Transforms existing text with tone modulation, grammar correction, and structural adjustments.
- **Smart Chat Assistant**: Contextual Q&A to brainstorm ideas, overcome writer's block, and gather SEO strategies.
- **Real-Time Streaming**: Vercel AI SDK streams token-by-token output for immediate visual feedback.

### 📚 Content & Document Management

- **Template Directory**: Built-in frameworks for blogs, social media, emails, advertising, and business documents.
- **Document Library**: Save and organize generated content seamlessly with auto-save capabilities.
- **Version History**: Keep track of previous iterations.
- **Export Options**: Download generated content as Markdown, HTML, or plain text.

### 📊 Dashboard & Personalization

- **Usage Analytics**: Real-time visualization of words generated, AI requests made, and token usage limits.
- **Profile Management**: Customize user preferences, account settings, and subscription states.
- **Full-Text Search**: Instantly locate past content by keyword or generation date.

### 🔐 Authentication & Subscription Management

- **Multi-Channel Auth**: Email/password and Google OAuth 2.0 integration via NextAuth.js.
- **Role-Based Access Control**: Safe segmentation between standard users and platform administrators.
- **Stripe Checkout**: Secure payment processing for premium feature unlocking.
- **Session Security**: JWT-based secure HTTP-only cookies.

### 📱 Responsive & Accessible Design

- **Mobile-First Approach**: Optimized from smartphones to large desktop screens.
- **Dark Mode Support**: Built-in theme switching with `next-themes`.
- **WCAG 2.1 Compliance**: Built on Radix primitives to ensure keyboard navigation and screen-reader accessibility.
- **Performance Optimized**: Heavy reliance on Next.js Server Components and dynamic imports.

---

## 🏗️ Software Architecture
<img width="1440" height="1520" alt="image" src="https://github.com/user-attachments/assets/4ed099a7-efce-4ef2-862a-75f6e3ed0f21" />


### Data Flow

1. **User Authentication**: NextAuth.js handles registration, login, and session persistence.
2. **AI Requests**: The React client dispatches prompts via Vercel AI SDK to Next.js API routes.
3. **Data Processing**: The API routes validate the session, check Prisma for usage limits, and construct the prompt.
4. **External Services**: The backend queries Groq for AI inference.
5. **Response Delivery**: A readable stream of tokens is returned to the client and rendered instantly.
6. **Persistence**: Finished documents and usage logs are safely committed to PostgreSQL.

---

## 🛠️ Tech Stack

### Frontend & Core Framework

| Technology | Version | Purpose |
|-----------|---------|---------|
| **Next.js** | 14.2.15 | React framework with App Router and Serverless API Routes |
| **React** | 18.x | Modern UI library with concurrent rendering |
| **TypeScript** | 5.x | Type-safe development with static type checking |
| **TailwindCSS** | 3.4.1 | Utility-first CSS framework for rapid UI development |
| **Shadcn UI** | 4.8.0 | Beautiful component library built on Radix primitives |
| **Framer Motion** | 12.x | Production-ready animations and transitions |
| **Vercel AI SDK** | 6.0.x | Unified AI abstraction with React streaming hooks |
| **Recharts** | 3.8.1 | Composable charting library for data visualization |
| **Lucide React** | 1.17.0 | Beautiful, consistent icon library |

### Backend & Database

| Technology | Version | Purpose |
|-----------|---------|---------|
| **Next.js APIs** | 14.2.15 | Serverless endpoints for secure business logic |
| **NextAuth.js** | 4.24.14 | Complete authentication and session management |
| **PostgreSQL** | 16.x | Robust relational database |
| **Prisma ORM** | 5.22.0 | Next-generation Node.js & TypeScript ORM |
| **bcryptjs** | 3.0.3 | Password hashing with salt rounds |

### External Services

| Service | Purpose | Integration |
|---------|---------|-------------|
| **Groq AI** | Inference Engine | LLaMA 3.3 70B model integration |
| **Stripe** | Payment Processing | Secure checkout sessions & webhooks |
| **Google OAuth** | Social Authentication | One-click sign-in |
| **Vercel** | Deployment Platform | Serverless hosting and edge functions |

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18.0.0 or higher)
- **npm** (v9.0.0 or higher)
- **Git** for version control
- **PostgreSQL Database** (local installation or cloud-hosted via Supabase/Neon)
- **Stripe** account ([test mode](https://dashboard.stripe.com/register))
- **Groq API** key ([free tier](https://console.groq.com/))

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/SiratimMChy/Writeflow-AI.git
cd Writeflow-AI/writeflow-ai-frontend
```

2. **Install dependencies**

```bash
npm install
```

3. **Set up environment variables**

Create a `.env` file in the `writeflow-ai-frontend` directory:

```env
DATABASE_URL=postgresql://user:password@localhost:5432/writeflow
DIRECT_URL=postgresql://user:password@localhost:5432/writeflow
NEXTAUTH_SECRET=your_super_secret_nextauth_string
NEXTAUTH_URL=http://localhost:3000
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GROQ_API_KEY=your_groq_api_key
STRIPE_SECRET_KEY=sk_test_...
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=pk_test_...
```

4. **Initialize the Database**

```bash
npx prisma generate
npx prisma db push
npx prisma db seed
```

5. **Start the development server**

```bash
npm run dev
```

6. **Open your browser**

Navigate to `http://localhost:3000` to see the application running.

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DATABASE_URL` | Prisma Connection Pool URL | Yes |
| `NEXTAUTH_SECRET` | Secret key for JWT signing | Yes |
| `NEXTAUTH_URL` | Application base URL | Yes |
| `GOOGLE_CLIENT_ID` | Google OAuth client ID | Optional |
| `GOOGLE_CLIENT_SECRET` | Google OAuth secret | Optional |
| `GROQ_API_KEY` | Groq AI API key | Yes |
| `STRIPE_SECRET_KEY` | Stripe secret key | Yes |
| `NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY`| Stripe publishable key | Yes |

---

## 📖 Usage

### Getting Started with WriteFlow AI

1. **Create Your Account**
   - Navigate to `/register`
   - Sign up with email/password or use Google OAuth

2. **Generate AI Content**
   - Head over to the **Draft Agent** in your dashboard.
   - Enter your requirements, tone, and desired template.
   - Watch the platform stream the final result instantly.

3. **Refine and Format**
   - Use the **Rewrite Agent** to condense, expand, or adjust the tone of your text.
   - Use the **Chat Assistant** for more complex requests.

4. **Manage Documents**
   - Click the "Save" button to commit drafts to your **Documents** library.
   - View, edit, and export them later.

5. **Monitor Your Quotas**
   - Access the **Analytics** page to track how many AI generation requests you have remaining on your current tier.

### Key Pages

- **`/`** - Landing page with hero, features, and pricing
- **`/login`** - User authentication
- **`/register`** - New user registration
- **`/explore`** - Public template library browser
- **`/dashboard`** - User dashboard overview
- **`/dashboard/draft`** - AI Draft Agent interface
- **`/dashboard/rewrite`** - AI Rewrite Agent interface
- **`/dashboard/chat`** - AI Chat Assistant
- **`/dashboard/documents`** - Document library
- **`/dashboard/analytics`** - Usage metrics and token limits

---

## 📁 Project Structure

WriteFlow AI consists of two main directories: `writeflow-ai-frontend` and `writeflow-ai-backend`.

```
writeflow-ai/
├── writeflow-ai-frontend/       # The primary Next.js Full-Stack Application
│   ├── public/                  # Static assets
│   ├── prisma/                  # Database definitions
│   │   ├── schema.prisma        # PostgreSQL Models
│   │   └── seed.ts              # Database seeder scripts
│   ├── src/
│   │   ├── app/                 # Next.js App Router
│   │   │   ├── (auth)/          # Authentication routes
│   │   │   ├── api/             # API Endpoints
│   │   │   │   ├── ai/          # Draft, Rewrite, and Chat endpoints
│   │   │   │   ├── auth/        # NextAuth handler
│   │   │   │   ├── billing/     # Stripe sessions
│   │   │   │   ├── documents/   # Document CRUD
│   │   │   │   └── settings/    # Profile management
│   │   │   ├── dashboard/       # Protected application workspace
│   │   │   ├── explore/         # Public pages
│   │   │   ├── globals.css      # Global Tailwind styles
│   │   │   └── layout.tsx       # Root layout
│   │   ├── components/          # React components
│   │   │   ├── auth/            # Login/Register UI
│   │   │   ├── dashboard/       # Sidebar, Header, Stats cards
│   │   │   ├── layouts/         # Shared wrappers
│   │   │   └── ui/              # Shadcn primitive components
│   │   ├── lib/                 # Utilities & configurations
│   │   │   ├── api.ts           # Axios base instances
│   │   │   ├── auth.ts          # NextAuth configuration
│   │   │   ├── groq.ts          # Groq SDK setup
│   │   │   ├── prisma.ts        # Prisma singleton
│   │   │   └── utils.ts         # Generic helpers
│   │   └── types/               # TypeScript definitions
│   ├── .env.example             # Environment template
│   ├── next.config.mjs          # Next.js bundler config
│   ├── package.json             # App dependencies
│   ├── tailwind.config.ts       # Tailwind CSS config
│   └── tsconfig.json            # TypeScript settings
│
├── writeflow-ai-backend/        # Node.js/Express Backend Service
│   ├── src/
│   │   ├── config/              # Server configurations
│   │   ├── middlewares/         # Express middlewares
│   │   ├── modules/             # Feature modules (e.g., document)
│   │   ├── types/               # TypeScript definitions
│   │   ├── app.ts               # Express application setup
│   │   ├── seed.ts              # Database seeder scripts
│   │   └── server.ts            # Server entry point
│   ├── .env.example             # Environment template
│   ├── package.json             # App dependencies
│   └── tsconfig.json            # TypeScript settings
│
└── README.md                    # Project documentation
```

---

## 🔌 API Documentation

WriteFlow AI provides a comprehensive API built directly into Next.js Serverless Routes. All endpoints return JSON responses.

### Base URL

- **Production**: `https://write-flow-ai-tau.vercel.app`
- **Development**: `http://localhost:3000`

### Authentication

Endpoints under `/api/` (excluding public webhooks) strictly require authentication via NextAuth.js secure cookies.

### AI Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `POST` | `/api/ai/draft` | Stream newly generated AI content | User |
| `POST` | `/api/ai/rewrite` | Stream structural transformations | User |
| `POST` | `/api/chat` | AI conversational completions | User |

### Document Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `GET` | `/api/documents` | Fetch user's saved documents | User |
| `POST` | `/api/documents` | Save a new generated document | User |
| `GET` | `/api/documents/:id` | Fetch specific document | User |
| `DELETE` | `/api/documents/:id` | Delete a document | User |

### Billing & User Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `GET` | `/api/dashboard/stats` | Fetch usage tracking statistics | User |
| `GET` | `/api/settings/profile` | Fetch active user profile | User |
| `POST` | `/api/billing/checkout` | Create Stripe checkout session | User |
| `POST` | `/api/webhooks/stripe` | Handle Stripe payment callbacks | None |

---

## 🌐 Deployment

### Vercel (Recommended)

WriteFlow AI is built for serverless, making Vercel the ideal deployment platform.

#### Deployment Steps

1. **Push your code to GitHub**
   ```bash
   git add .
   git commit -m "Ready for production"
   git push origin main
   ```

2. **Connect to Vercel**
   - Visit [vercel.com](https://vercel.com)
   - Click "New Project" and import your repository.
   - **Crucial:** Set the **Root Directory** to `writeflow-ai-frontend`.

3. **Configure Environment Variables**
   - Add all required secrets (`DATABASE_URL`, `NEXTAUTH_SECRET`, `GROQ_API_KEY`, etc.) inside the Vercel Settings panel.

4. **Deploy**
   - Vercel automatically detects Next.js.
   - Set the build command to: `npx prisma generate && next build`
   - Click "Deploy". Your app will automatically build and deploy.

### Alternative Deployment Options

#### Docker Deployment

```dockerfile
FROM node:20-alpine
WORKDIR /app
COPY writeflow-ai-frontend/package*.json ./
RUN npm ci
COPY writeflow-ai-frontend/ .
RUN npx prisma generate
RUN npm run build
EXPOSE 3000
CMD ["npm", "start"]
```

Build and run:
```bash
docker build -t writeflow-ai .
docker run -p 3000:3000 --env-file .env writeflow-ai
```

---

## 🔒 Security & Best Practices

### Security Features

#### Authentication & Authorization
- **NextAuth.js**: Industry-standard authentication with HTTP-only, secure session management.
- **Role-Based Access Control**: Prevents standard users from accessing admin analytics or template creation tools.
- **Password Security**: Standard bcrypt hashing protocols executed safely server-side.
- **Protected API Routes**: Backend endpoints instantly reject unauthenticated requests.

#### Data Protection
- **HTTPS Only**: All traffic heavily encrypted via TLS/SSL.
- **Database Safety**: Prisma ORM executes parameterized queries by default, protecting entirely against SQL Injection.
- **Stripe PCI Compliance**: Level 1 compliance for payment processing.

#### AI Integrity
- **Rate Limiting**: AI endpoints check Prisma `AIUsageLog` rows to prevent users from exceeding monthly AI token quotas and abusing the Groq API.
- **Prompt Sanitization**: System prompts strictly bound the LLM's behavioral output to prevent prompt injection.

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

### How to Contribute

1. **Fork the Project**
2. **Clone Your Fork**
3. **Create a Feature Branch** (`git checkout -b feature/AmazingFeature`)
4. **Make Your Changes** and document them cleanly.
5. **Commit Your Changes** (`git commit -m 'Add some AmazingFeature'`)
6. **Push to Your Fork** (`git push origin feature/AmazingFeature`)
7. **Open a Pull Request**

---

## 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

---

## 📧 Contact

**Project Maintainer**: Siratim Mustakim Chowdhury

- 📧 **Email**: [chowdhurysiratimmustakim@gmail.com](mailto:chowdhurysiratimmustakim@gmail.com)
- 🐙 **GitHub**: [@SiratimMChy](https://github.com/SiratimMChy)
- 💼 **LinkedIn**: [Siratim Mustakim Chowdhury](https://www.linkedin.com/in/siratim-mustakim-chowdhury/)

---

## 🙏 Acknowledgments

### Technologies & Libraries

- [Next.js](https://nextjs.org/) - React framework with App Router
- [React](https://react.dev/) - UI library for building interfaces
- [TypeScript](https://www.typescriptlang.org/) - Type-safe JavaScript
- [Prisma](https://www.prisma.io/) - Next-generation Node.js and TypeScript ORM
- [PostgreSQL](https://www.postgresql.org/) - Relational database
- [NextAuth.js](https://next-auth.js.org/) - Authentication solution
- [Stripe](https://stripe.com/) - Payment processing
- [Groq](https://groq.com/) - LLaMA AI inference engine
- [TailwindCSS](https://tailwindcss.com/) - CSS framework
- [Shadcn UI](https://ui.shadcn.com/) - Beautiful, accessible components

---

## 📊 Project Statistics

- **Stack**: Next.js + React + TypeScript + Prisma + PostgreSQL + Stripe + Groq AI
- **Total Lines of Code**: 20,000+
- **React Components**: 40+
- **API Endpoints**: 15+
- **PostgreSQL Tables**: 7
- **Supported Devices**: Desktop, Tablet, Mobile
- **Deployment Platforms**: Vercel, Docker, Self-hosted
- **Authentication Methods**: Email/Password, Google OAuth

---

<div align="center">

**Made by Siratim Mustakim Chowdhury**

[![GitHub](https://img.shields.io/badge/GitHub-SiratimMChy-181717?style=flat&logo=github)](https://github.com/SiratimMChy)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Siratim%20Mustakim-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/siratim-mustakim-chowdhury/)
[![Email](https://img.shields.io/badge/Email-chowdhurysiratimmustakim@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chowdhurysiratimmustakim@gmail.com)

</div>
