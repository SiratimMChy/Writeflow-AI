# ✨ WriteFlow AI - Next.js AI-Powered Content Creation Platform

<div align="center">

**A modern, full-stack Next.js application for AI-powered content generation and management**

![Next.js](https://img.shields.io/badge/Next.js-14.2.15-black?style=for-the-badge&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=white)

[![TailwindCSS](https://img.shields.io/badge/Tailwind-3.4.1-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer%20Motion-12.40.0-FF0055?style=flat&logo=framer&logoColor=white)](https://www.framer.com/motion/)
[![Groq](https://img.shields.io/badge/Groq-LLaMA%203.3%2070B-orange?style=flat)](https://groq.com/)
[![Vercel AI SDK](https://img.shields.io/badge/Vercel%20AI%20SDK-6.0-000000?style=flat&logo=vercel&logoColor=white)](https://sdk.vercel.ai/)

<div align="center">
<a href="https://writeflow-ai.vercel.app/" target="_blank">

![Live Demo](https://img.shields.io/badge/WRITEFLOW%20AI-LIVE%20DEMO-6366F1?style=for-the-badge&logo=firefox-browser&logoColor=white&labelColor=111827)

</a>
</div>

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#️-tech-stack)
- [Getting Started](#-getting-started)
- [Environment Setup](#-environment-setup)
- [Project Structure](#-project-structure)
- [AI Agent System](#-ai-agent-system)
- [API Integration](#-api-integration)
- [Deployment](#-deployment)
- [Demo Credentials](#-demo-credentials)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Overview

**WriteFlow AI** is a next-generation AI-powered content creation platform that transforms the writing workflow for professionals, marketers, and content creators. Built with cutting-edge technologies, it provides specialized AI agents for drafting, rewriting, and interactive content assistance—all within a sleek, premium dashboard experience.

### Why WriteFlow AI?

- 🚀 **50+ Pre-optimized Templates** - Industry-proven frameworks for blogs, ads, social media, and email campaigns
- 🤖 **Specialized AI Agents** - Dedicated agents for drafting, rewriting, and chat assistance
- ⚡ **Real-time Streaming** - Watch content generate in real-time with smooth text streaming
- 🎨 **Premium UI/UX** - Beautifully designed interface with Framer Motion animations
- 📊 **Advanced Analytics** - Track word counts, document metrics, and productivity insights
- 👥 **Team Collaboration** - Multi-user workspace with role-based access control
- 🔒 **Secure by Design** - JWT authentication with bcrypt encryption

### 🔗 Live Application

**Production URL:** [https://writeflow-ai.vercel.app](https://writeflow-ai.vercel.app)

---

## ✨ Key Features

### 🎨 **User Interface**
- **Modern Dark Theme** - Sophisticated black and violet gradient design
- **Responsive Layout** - Fully optimized for desktop, tablet, and mobile devices
- **Smooth Animations** - Framer Motion-powered transitions and micro-interactions
- **Interactive Dashboard** - Real-time statistics and quick action cards
- **Premium Components** - Built with Radix UI and shadcn/ui primitives

### 🤖 **AI-Powered Content Generation**

#### 1. **Draft Agent** 
Generate high-quality, long-form content from scratch:
- Multiple tone options (Professional, Casual, Enthusiastic, Informative, Persuasive)
- Keyword integration for SEO optimization
- Template-based generation with 50+ presets
- Real-time streaming with word-by-word output
- Instant save and copy functionality

#### 2. **Rewrite Agent**
Transform and enhance existing content:
- Multiple rewriting modes (Expand, Shorten, Fix Grammar, Change Tone)
- Preserve original meaning while improving readability
- Style transformation (Formal ↔ Casual)
- Grammar and spelling correction
- Sentence structure optimization

#### 3. **Chat Assistant**
Interactive AI partner for brainstorming:
- Context-aware conversations
- Content strategy suggestions
- Research and ideation support
- Writing tips and best practices
- Multi-turn dialogue with memory

### 📚 **Template Library**
- **50+ Templates** across categories: Blog, Social Media, Email, Ads, SEO
- **Smart Filtering** by category, rating, and popularity
- **Search Functionality** with real-time results
- **Usage Statistics** showing popularity metrics
- **Star Ratings** from community feedback

### 📊 **Dashboard & Analytics**
- **Document Management** - Create, save, edit, and organize content
- **Word Count Tracking** - Monitor total and weekly word generation
- **Time Saved Calculator** - Estimated hours saved vs. manual writing
- **Recent Activity** - Quick access to latest documents
- **Quick Actions** - Shortcut cards for common tasks

### 👤 **User Management**
- **Secure Authentication** - JWT-based auth with httpOnly cookies
- **Profile Management** - Update personal information and preferences
- **Document History** - Full audit trail of all generated content
- **Settings Panel** - Customize writing preferences and AI behavior

### 🔐 **Admin Panel** (Role-Based Access)
- **User Management** - View, edit, and moderate user accounts
- **Template Management** - Add, modify, and delete template library items
- **Analytics Dashboard** - System-wide usage statistics and trends
- **Review Moderation** - Approve or reject user-submitted reviews
- **Site Settings** - Configure maintenance mode and system parameters

---

## 🛠️ Tech Stack

### **Frontend**
| Technology | Purpose | Version |
|------------|---------|---------|
| [Next.js](https://nextjs.org/) | React Framework (App Router) | 14.2.15 |
| [TypeScript](https://www.typescriptlang.org/) | Type Safety | 5.x |
| [Tailwind CSS](https://tailwindcss.com/) | Utility-First Styling | 3.4.1 |
| [Framer Motion](https://www.framer.com/motion/) | Animation Library | 12.40.0 |
| [Radix UI](https://www.radix-ui.com/) | Headless Component Primitives | Various |
| [shadcn/ui](https://ui.shadcn.com/) | Component Library | 4.8.0 |
| [Lucide React](https://lucide.dev/) | Icon Library | 1.17.0 |

### **AI & Data Handling**
| Technology | Purpose | Version |
|------------|---------|---------|
| [AI SDK (Vercel)](https://sdk.vercel.ai/) | Streaming AI Responses | 6.0.191 |
| [Groq SDK](https://groq.com/) | LLM API Integration | 1.2.1 |
| [Axios](https://axios-http.com/) | HTTP Client | 1.16.1 |

### **State & UI Utilities**
| Technology | Purpose |
|------------|---------|
| [Sonner](https://sonner.emilkowal.ski/) | Toast Notifications |
| [cookies-next](https://www.npmjs.com/package/cookies-next) | Cookie Management |
| [clsx](https://github.com/lukeed/clsx) | Conditional Classnames |
| [Recharts](https://recharts.org/) | Data Visualization |

### **Development Tools**
- **ESLint** - Code linting and quality
- **PostCSS** - CSS processing
- **Docker** - Containerization support
- **Docker Compose** - Multi-container orchestration

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:
- **Node.js** (v18.0.0 or higher)
- **npm** or **yarn** (latest version)
- **Git** (for cloning the repository)

### Installation Steps

#### 1️⃣ Clone the Repository

```bash
git clone https://github.com/SiratimMChy/WriteFlowAI.git
cd WriteFlowAI/writeflow-ai
```

#### 2️⃣ Install Dependencies

```bash
npm install
# or
yarn install
```

#### 3️⃣ Configure Environment Variables

Create a `.env.local` file in the root directory:

```env
# Backend API Configuration
NEXT_PUBLIC_API_URL=https://writeflowai-backend.onrender.com/api

# Groq API Key (Required for AI generation)
GROQ_API_KEY=your-groq-api-key-here

# NextAuth Configuration (if using authentication)
NEXTAUTH_SECRET=your-nextauth-secret-key
NEXTAUTH_URL=http://localhost:3000

# Optional: Google OAuth (for social login)
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret

# Optional: Database Connection (if running locally)
DATABASE_URL=postgresql://username:password@localhost:5432/writeflow
DIRECT_URL=postgresql://username:password@localhost:5432/writeflow
```

**Get Your Groq API Key:**
1. Visit [Groq Console](https://console.groq.com/)
2. Sign up or log in
3. Navigate to API Keys section
4. Generate a new API key

#### 4️⃣ Run the Development Server

```bash
npm run dev
# or
yarn dev
```

The application will be available at **http://localhost:3000**

#### 5️⃣ Build for Production

```bash
npm run build
npm run start
# or
yarn build
yarn start
```

---

## 🔧 Environment Setup

### Required Environment Variables

| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| `NEXT_PUBLIC_API_URL` | Backend API base URL | ✅ Yes | - |
| `GROQ_API_KEY` | Groq LLM API key | ✅ Yes | - |
| `NEXTAUTH_SECRET` | NextAuth JWT secret | ⚠️ Recommended | - |
| `NEXTAUTH_URL` | Application base URL | ⚠️ Recommended | http://localhost:3000 |

### Optional Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GOOGLE_CLIENT_ID` | Google OAuth client ID | ❌ No |
| `GOOGLE_CLIENT_SECRET` | Google OAuth client secret | ❌ No |
| `DATABASE_URL` | PostgreSQL connection string (pooled) | ❌ No |
| `DIRECT_URL` | PostgreSQL direct connection string | ❌ No |

**Get Your Groq API Key:**
1. Visit [Groq Console](https://console.groq.com/)
2. Sign up or log in to your account
3. Navigate to the API Keys section
4. Click "Create API Key" and copy it
5. Add it to your `.env.local` file

---

## 📁 Project Structure

```
writeflow-ai/
├── src/
│   ├── app/                          # Next.js App Router
│   │   ├── (auth)/                   # Authentication routes
│   │   │   ├── login/
│   │   │   ├── register/
│   │   │   └── forgot-password/
│   │   ├── dashboard/                # Protected dashboard routes
│   │   │   ├── page.tsx              # Dashboard home
│   │   │   ├── draft/                # Draft Agent UI
│   │   │   ├── rewrite/              # Rewrite Agent UI
│   │   │   ├── chat/                 # Chat Assistant UI
│   │   │   ├── documents/            # Document management
│   │   │   ├── templates/            # Template browser
│   │   │   ├── analytics/            # User analytics
│   │   │   ├── profile/              # User profile
│   │   │   ├── settings/             # Account settings
│   │   │   └── admin/                # Admin panel
│   │   │       ├── users/
│   │   │       ├── templates/
│   │   │       ├── analytics/
│   │   │       └── reviews/
│   │   ├── about/                    # About page
│   │   ├── blog/                     # Blog listing
│   │   ├── contact/                  # Contact form
│   │   ├── explore/                  # Template exploration
│   │   ├── privacy/                  # Privacy policy
│   │   ├── terms/                    # Terms of service
│   │   ├── layout.tsx                # Root layout
│   │   ├── page.tsx                  # Landing page
│   │   └── globals.css               # Global styles
│   ├── components/                   # React components
│   │   ├── ui/                       # shadcn/ui components
│   │   ├── navbar.tsx                # Navigation bar
│   │   ├── footer.tsx                # Footer component
│   │   ├── dashboard-sidebar.tsx     # Dashboard navigation
│   │   ├── draft-agent-client.tsx    # Draft Agent UI
│   │   ├── rewrite-agent-client.tsx  # Rewrite Agent UI
│   │   ├── chat-agent-client.tsx     # Chat Assistant UI
│   │   ├── template-card.tsx         # Template card component
│   │   ├── auth-provider.tsx         # Auth context provider
│   │   └── providers.tsx             # App-wide providers
│   └── lib/                          # Utility functions
│       ├── api.ts                    # Axios instance & interceptors
│       ├── groq.ts                   # Groq SDK configuration
│       ├── utils.ts                  # Helper functions
│       └── avatar.ts                 # Avatar utilities
├── public/                           # Static assets
│   ├── team/                         # Team member photos
│   └── favicon.ico
├── .env.example                      # Environment template
├── next.config.mjs                   # Next.js configuration
├── tailwind.config.ts                # Tailwind CSS configuration
├── tsconfig.json                     # TypeScript configuration
├── docker-compose.yml                # Docker setup
├── Dockerfile                        # Container definition
└── package.json                      # Project dependencies
```

---

## 🤖 AI Agent System

WriteFlow AI features three specialized AI agents powered by **Groq's LLaMA 3.3 70B** model:

### 1. **Draft Agent** (`/dashboard/draft`)

**Purpose:** Generate original content from scratch

**API Endpoint:** `POST /api/ai/draft`

**Configuration:**
```typescript
{
  prompt: string;          // User's topic or brief
  tone: string;            // Professional | Casual | Enthusiastic | Informative | Persuasive
  keywords?: string;       // Optional SEO keywords
  templateId?: string;     // Optional template context
}
```

**Features:**
- Real-time streaming response
- Automatic word count
- Save to document library
- Copy to clipboard
- Template integration

**Implementation Highlights:**
- Uses Vercel AI SDK's `useCompletion` hook
- Streams tokens for smooth rendering
- Automatic error handling with toast notifications
- JWT authentication via Axios interceptor

### 2. **Rewrite Agent** (`/dashboard/rewrite`)

**Purpose:** Transform and improve existing content

**API Endpoint:** `POST /api/ai/rewrite`

**Modes:**
- **Expand** - Add more detail and depth
- **Shorten** - Condense while preserving meaning
- **Fix Grammar** - Correct errors and improve syntax
- **Change Tone** - Transform style (Formal ↔ Casual)

**Configuration:**
```typescript
{
  originalText: string;    // Content to rewrite
  mode: string;            // Expand | Shorten | Fix Grammar | Change Tone
  targetTone?: string;     // Required if mode = "Change Tone"
}
```

### 3. **Chat Assistant** (`/dashboard/chat`)

**Purpose:** Interactive brainstorming and content advice

**API Endpoint:** `POST /api/ai/chat`

**Features:**
- Multi-turn conversations
- Context retention
- Markdown formatting
- Code syntax highlighting
- Message history

**Use Cases:**
- Content strategy planning
- Topic ideation
- SEO optimization tips
- Writing technique guidance

---

## 📡 API Integration

### Base URL
```
Production: https://writeflowai-backend.onrender.com/api
```

### Authentication

All protected endpoints require a JWT token:

```typescript
Headers: {
  'Authorization': 'Bearer <your-jwt-token>',
  'Content-Type': 'application/json'
}
```

### Endpoints Overview

#### 🔑 **Authentication**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/auth/register` | Create new user account | ❌ No |
| POST | `/auth/login` | Authenticate and get JWT | ❌ No |
| POST | `/auth/logout` | Invalidate session | ✅ Yes |
| GET | `/auth/profile` | Get current user details | ✅ Yes |
| PUT | `/auth/profile` | Update user profile | ✅ Yes |

**Example Registration:**
```typescript
POST /auth/register
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "SecurePass123!"
}
```

#### 📄 **Documents**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/documents` | List user's documents (paginated) | ✅ Yes |
| POST | `/documents/save` | Save generated content | ✅ Yes |
| GET | `/documents/:id` | Get specific document | ✅ Yes |
| PUT | `/documents/:id` | Update document | ✅ Yes |
| DELETE | `/documents/:id` | Delete document | ✅ Yes |

**Example Document Save:**
```typescript
POST /documents/save
{
  "title": "My Blog Post",
  "content": "Generated content here...",
  "status": "draft",
  "type": "draft",
  "wordCount": 1250,
  "templateId": "seo-blog-post"
}
```

#### 🤖 **AI Agents**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/ai/draft` | Generate new content (streaming) | ✅ Yes |
| POST | `/ai/rewrite` | Rewrite existing content (streaming) | ✅ Yes |
| POST | `/ai/chat` | Chat with AI assistant (streaming) | ✅ Yes |

**Example Draft Request:**
```typescript
POST /ai/draft
{
  "prompt": "Write a blog post about AI in healthcare",
  "tone": "Professional",
  "keywords": "artificial intelligence, medical diagnosis, patient care",
  "templateId": "blog-post"
}
```

#### 📚 **Templates**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/items` | Get template library (with filters) | ❌ No |
| GET | `/items/:id` | Get specific template | ❌ No |
| POST | `/items` | Create template (admin only) | ✅ Yes (Admin) |
| PUT | `/items/:id` | Update template (admin only) | ✅ Yes (Admin) |
| DELETE | `/items/:id` | Delete template (admin only) | ✅ Yes (Admin) |

**Query Parameters:**
```typescript
GET /items?category=Blog&sort=popular&page=1&limit=12&search=SEO
```

#### 📊 **Analytics**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/dashboard/stats` | User statistics | ✅ Yes |
| GET | `/dashboard/public-stats` | Public platform stats | ❌ No |
| GET | `/dashboard/admin/analytics` | System-wide analytics | ✅ Yes (Admin) |

**Example Stats Response:**
```json
{
  "success": true,
  "data": {
    "totalDocuments": 42,
    "totalWords": 35000,
    "documentsThisWeek": 7,
    "wordsThisWeek": 5200
  }
}
```

#### 👥 **Admin Panel**

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/dashboard/admin/users` | List all users | ✅ Yes (Admin) |
| PUT | `/dashboard/admin/users/:id` | Update user status | ✅ Yes (Admin) |
| DELETE | `/dashboard/admin/users/:id` | Delete user | ✅ Yes (Admin) |
| GET | `/dashboard/admin/reviews` | Manage reviews | ✅ Yes (Admin) |
| PUT | `/dashboard/admin/reviews/:id` | Approve/reject review | ✅ Yes (Admin) |
| GET | `/settings` | Get site settings | ✅ Yes (Admin) |
| PUT | `/settings` | Update site settings | ✅ Yes (Admin) |

### Error Handling

All API responses follow this structure:

```typescript
// Success
{
  "success": true,
  "data": { ... },
  "meta": { ... }  // Optional pagination info
}

// Error
{
  "success": false,
  "error": {
    "message": "Error description",
    "code": "ERROR_CODE"
  }
}
```

---

## 🚢 Deployment

### Vercel (Recommended)

WriteFlow AI is optimized for Vercel deployment:

1. **Fork/Clone** the repository
2. **Import** to Vercel dashboard
3. **Configure** environment variables:
   - `NEXT_PUBLIC_API_URL`
   - `GROQ_API_KEY`
   - `NEXTAUTH_SECRET`
   - `NEXTAUTH_URL`
4. **Deploy** with one click

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/SiratimMChy/WriteFlowAI)

### Docker

Run with Docker Compose:

```bash
docker-compose up -d
```

This starts:
- **Next.js app** on port 3000
- **PostgreSQL database** on port 5432

**Custom Docker Build:**
```bash
docker build -t writeflow-ai .
docker run -p 3000:3000 --env-file .env writeflow-ai
```

### Other Platforms

WriteFlow AI can be deployed to any platform supporting Node.js:
- **Netlify** (with Next.js plugin)
- **Railway**
- **Render**
- **AWS Amplify**
- **Digital Ocean App Platform**

---

## 🔑 Demo Credentials

Test the application with pre-configured accounts:

### 👤 **Regular User Account**
```
Email: user@writeflow.com
Password: 123456
```
**Access:** Draft, Rewrite, Chat agents, Document management, Profile settings

### 🛡️ **Administrator Account**
```
Email: admin@writeflow.com
Password: admin123
```
**Access:** All user features + Admin panel (User management, Template management, Analytics, Review moderation)

> ⚠️ **Note:** These are demo credentials for testing purposes only. Change them in production environments.

---

## 🤝 Contributing

Contributions are welcome and greatly appreciated! Here's how you can contribute:

### How to Contribute

1. **Fork the Repository**
   - Click the "Fork" button at the top right of the repository page

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/your-username/WriteFlowAI.git
   cd WriteFlowAI/writeflow-ai
   ```

3. **Create a Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

4. **Make Your Changes**
   - Write clean, readable code
   - Follow existing code style and conventions
   - Add comments for complex logic

5. **Test Your Changes**
   - Test thoroughly across different devices
   - Ensure no existing functionality is broken

6. **Commit Your Changes**
   ```bash
   git add .
   git commit -m 'Add some AmazingFeature'
   ```

7. **Push to Your Fork**
   ```bash
   git push origin feature/AmazingFeature
   ```

8. **Open a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your feature branch
   - Provide a clear description of your changes

### Contribution Guidelines

- **Code Style**: Follow existing code conventions and formatting
- **Commit Messages**: Write clear, descriptive commit messages
- **Documentation**: Update README and comments for new features
- **Testing**: Ensure all features work as expected
- **Pull Requests**: Keep PRs focused on a single feature or fix
- **Issues**: Check existing issues before creating new ones

### Areas for Contribution

- 🐛 Bug fixes and error handling improvements
- ✨ New features and AI agent enhancements
- 📝 Documentation improvements
- 🎨 UI/UX enhancements and animations
- ⚡ Performance optimizations
- 🧪 Test coverage improvements
- 🌐 Internationalization (i18n)
- ♿ Accessibility improvements
- 📱 Mobile responsiveness enhancements
- � Next.js best practices implementation

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### MIT License Summary

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software.

---

## 📧 Contact
- 📧 **Email**: [chowdhurysiratimmustakim@gmail.com](mailto:chowdhurysiratimmustakim@gmail.com)
- 🐙 **GitHub**: [@SiratimMChy](https://github.com/SiratimMChy)
- 💼 **LinkedIn**: [Siratim Mustakim Chowdhury](https://www.linkedin.com/in/siratim-mustakim-chowdhury/)

---

## 🌟 Acknowledgments

- [Vercel AI SDK](https://sdk.vercel.ai/) for streaming AI responses
- [Groq](https://groq.com/) for blazing-fast LLM inference
- [shadcn/ui](https://ui.shadcn.com/) for beautiful component primitives
- [Framer Motion](https://www.framer.com/motion/) for smooth animations
- The open-source community for amazing tools and libraries

---

## 📞 Support

- 📧 Email: support@writeflow.ai
- 🌐 Website: [https://writeflow-ai.vercel.app](https://writeflow-ai.vercel.app)
- 💬 Discord: [Join our community](#)
- 🐦 Twitter: [@WriteFlowAI](#)

---

<div align="center">

**⭐ Star this repo if you find it helpful! ⭐**

Made with ❤️ by Siratim Mustakim Chowdhury

[⬆ Back to Top](#writeflow-ai-)

</div>
