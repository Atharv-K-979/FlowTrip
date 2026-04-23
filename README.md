# 🗺️ FlowTrip - Unified Urban Mobility Intelligence Platform

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js Version](https://img.shields.io/badge/node-%3E%3D18.0.0-brightgreen)](https://nodejs.org)
[![React Version](https://img.shields.io/badge/react-18.2.0-blue)](https://react.dev)
[![Status: Production Ready](https://img.shields.io/badge/Status-Production%20Ready-success)](https://github.com)

---


## 🚀 Overview

**FlowTrip** is an AI-powered unified urban mobility platform that integrates multiple transport modes (walking, buses, trains, metros, cabs) into a single intelligent journey planning application.

Instead of juggling multiple apps for different transport modes, FlowTrip provides:
- **One unified platform** for all transport modes
- **Intelligent journey planning** with multiple optimization options
- **Real-time tracking** of your complete journey
- **AI-powered chatbot** for 24/7 assistance
- **Predictive intelligence** for delays, crowds, and weather
- **Confidence scoring** for journey reliability

---

## ✨ Screenshot's

<p align="center">
  <img src="public/image(1).png" alt="Boot Sequence" width="100%" style="border-radius: 20px;" />
</p>

<br />

<!-- <h3 align="center">2. Main Interface</h3> -->
<p align="center">
  <img src="public/image(2).png" alt="Landing Page" width="100%" style="border-radius: 10px;" />
</p>

<br />

<!-- <h3 align="center">3. Registration & System Lockdown</h3> -->
<p align="center">
  <img src="public/image(3).png" alt="Registration Form" width="80%" style="border-radius: 10px; display: inline-block;" />
</p>

<p align="center">
  <img src="public/image(4).png" alt="Lockdown Mode" width="60%" style="border-radius: 10px; display: inline-block;" /> 
</p>

---

### 🎯 Problem Statement

Urban commuters in Indian cities rely on multiple transport modes functioning in isolation. Commuters must:
- Use different apps for buses, trains, metros, and cabs
- Piece together fragmented information from multiple sources
- Manually synchronize timings and transfers
- Deal with uncertainty about delays and disruptions

**FlowTrip solves this** by providing end-to-end journey intelligence.

---

## ✨ Features

### 🎯 Core Features

#### 1. **Unified Journey Planning**
- Plan journeys using any combination of transport modes
- Get multiple options (Fastest, Cheapest, Most Reliable)
- See confidence scores for each option
- Real-time journey monitoring

#### 2. **Interactive Map**
- Visual route display with color-coded transport modes
- Custom markers for starts, transfers, and destinations
- Segment highlighting on hover/click
- Automatic route fitting on map load
- Touch-friendly on mobile devices

#### 3. **Journey Options**
```
Three optimization strategies:
├─ Fastest    (Minimize travel time)
├─ Cheapest   (Minimize cost)
└─ Reliable   (Maximize on-time probability)
```

#### 4. **Metrics Display**
- ⏰ Duration (in minutes)
- 💰 Cost (in rupees/dollars)
- ✅ Reliability Score (0-100)
- 🌱 CO₂ Saved (environmental impact)

#### 5. **AI Chatbot**
- Real-time journey assistance
- Route recommendations
- Booking help
- Accessibility support
- Multi-language support
- 24/7 availability

#### 6. **Predictive Intelligence**
- Traffic predictions
- Crowd level forecasting
- Delay predictions
- Weather impact analysis
- Reliability scoring

#### 7. **Real-Time Updates**
- Live location tracking
- Segment completion notifications
- Alert notifications
- ETA updates
- Crowd level updates

#### 8. **Responsive Design**
- Desktop (1440px+)
- Tablet (768px+)
- Mobile (375px+)
- Touch-friendly controls
- Optimized performance

---

## 🛠️ Tech Stack

### Frontend
```
Framework:     React 18.2.0
Styling:       Tailwind CSS 3.x
Animations:    Framer Motion 10.x
Mapping:       Leaflet.js + React-Leaflet
State:         Zustand 4.x
Routing:       React Router v6
Forms:         React Hook Form + Zod
Icons:         Lucide React
Charts:        Recharts
HTTP Client:   Axios
```

### Backend
```
Runtime:       Node.js 18+
Framework:     Express.js 4.x
Real-time:     Socket.io 4.x
Database:      PostgreSQL (Supabase)
Cache:         Redis
Authentication: JWT (Supabase Auth)
Validation:    Joi / Zod
Logging:       Winston / Pino
```

### Database & Auth
```
Primary DB:    Supabase PostgreSQL
Vector DB:     pgvector (embeddings)
File Storage:  Supabase Storage
Auth:          Supabase JWT
Row Security:  RLS Policies
Real-time:     Supabase Realtime
```

### AI & ML
```
Chatbot:       OpenAI GPT-4
Embeddings:    OpenAI Embeddings API
Predictions:   PyTorch + Scikit-learn
NLP:           Hugging Face Transformers
```

### DevOps & Deployment
```
Container:     Docker
Frontend:      Vercel
Backend:       Railway / AWS EC2
Database:      Supabase
CI/CD:         GitHub Actions
Monitoring:    Sentry + LogRocket
```

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have:
- **Node.js** 18+ ([Download](https://nodejs.org))
- **npm** or **yarn** package manager
- **Git** for version control
- **Supabase Account** ([Sign up](https://supabase.com))
- **OpenAI API Key** ([Get key](https://platform.openai.com))
- **Python 3.9+** (for ML models)

### Quick Start (5 minutes)

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/flowtrip.git
cd flowtrip

# 2. Install dependencies
npm install

# 3. Set up environment variables
cp .env.example .env.local
# Edit .env.local with your API keys

# 4. Start development server
npm run dev

# 5. Open http://localhost:5173
```

---

## 📦 Installation

### Detailed Setup Guide

#### Step 1: Clone Repository

```bash
git clone https://github.com/yourusername/flowtrip.git
cd flowtrip
```

#### Step 2: Set Up Frontend

```bash
cd frontend

# Install dependencies
npm install

# Create environment file
cp .env.example .env.local

# Edit .env.local
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
VITE_GOOGLE_MAPS_API_KEY=your_google_maps_key
```

#### Step 3: Set Up Backend

```bash
cd ../backend

# Install dependencies
npm install

# Create environment file
cp .env.example .env

# Edit .env
SUPABASE_URL=your_supabase_url
SUPABASE_SERVICE_KEY=your_service_key
OPENAI_API_KEY=your_openai_key
GOOGLE_MAPS_API_KEY=your_google_maps_key
JWT_SECRET=your_jwt_secret
DATABASE_URL=postgresql://user:password@host/db
REDIS_URL=redis://localhost:6379
PORT=3001
NODE_ENV=development
```

#### Step 4: Set Up Database

```bash
# Log into Supabase
# Create new project
# Get connection string

# Run migrations
npx supabase migration up

# Seed sample data
npm run seed
```

#### Step 5: Set Up ML Models (Optional)

```bash
# Create Python virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install Python dependencies
pip install -r requirements.txt

# Start ML service
python main.py
```

#### Step 6: Start Development

```bash
# Terminal 1: Frontend
cd frontend
npm run dev
# http://localhost:5173

# Terminal 2: Backend
cd backend
npm start
# http://localhost:3001

# Terminal 3: ML Service (optional)
cd ml-service
python main.py
# Running on port 5000
```

---

## 🏛️ Architecture

### System Architecture

```
┌─────────────────┐
│  Frontend SPA   │
│  (React 18)     │
└────────┬────────┘
         │
    HTTPS/WebSocket
         │
┌────────▼─────────────────┐
│  Backend API              │
│  (Express.js + Socket.io) │
└────────┬─────────────────┘
         │
    ┌────┴──────┬─────────┬──────────┐
    │            │         │          │
    ▼            ▼         ▼          ▼
┌─────────┐ ┌────────┐ ┌──────┐ ┌──────────┐
│Supabase │ │Redis   │ │OpenAI│ │External  │
│PostgreSQL│ │Cache   │ │GPT-4 │ │APIs      │
└─────────┘ └────────┘ └──────┘ └──────────┘
```

### Component Architecture

```
App
├─ Header
├─ Navigation
├─ Pages
│  ├─ Home
│  │  ├─ HeroSection
│  │  ├─ FeaturesSection
│  │  └─ CTASection
│  ├─ Journey
│  │  ├─ JourneyPlanner
│  │  │  ├─ JourneyOptionsPanel
│  │  │  ├─ MetricsDisplay
│  │  │  ├─ JourneyTimeline
│  │  │  ├─ SegmentsList
│  │  │  └─ MapVisualization
│  │  └─ Chat
│  ├─ Dashboard
│  └─ Admin
└─ Footer
```

### Data Flow

```
User Input
    ↓
Frontend Component
    ↓
API Request (Axios)
    ↓
Backend Controller
    ↓
Service Layer
    ├─ Journey Service
    ├─ Prediction Service
    └─ AI Service
    ↓
Database (Supabase)
    ↓
Response
    ↓
Frontend Update (Zustand)
    ↓
UI Re-render
```

---

## ⚙️ Configuration

### Environment Variables

#### Frontend (.env.local)
```env
# Supabase
VITE_SUPABASE_URL=https://xxxxx.supabase.co
VITE_SUPABASE_ANON_KEY=eyJhbGciOi...

# Google Maps
VITE_GOOGLE_MAPS_API_KEY=AIzaSy...

# API
VITE_API_URL=http://localhost:3001/api

# Features
VITE_ENABLE_ANALYTICS=true
VITE_ENABLE_SENTRY=false
VITE_LOG_LEVEL=debug
```

#### Backend (.env)
```env
# Supabase
SUPABASE_URL=https://xxxxx.supabase.co
SUPABASE_SERVICE_KEY=eyJhbGciOi...

# OpenAI
OPENAI_API_KEY=sk-proj-xxx

# Database
DATABASE_URL=postgresql://user:pass@host/db

# Cache
REDIS_URL=redis://localhost:6379

# Server
PORT=3001
NODE_ENV=development

# Auth
JWT_SECRET=your_super_secret_key

# External APIs
GOOGLE_MAPS_API_KEY=AIzaSy...
WEATHER_API_KEY=xxx

# Logging
LOG_LEVEL=debug
```

### Feature Flags

```javascript
// config/features.js
export const features = {
  ENABLE_CHATBOT: true,
  ENABLE_PREDICTIONS: true,
  ENABLE_REAL_TIME: true,
  ENABLE_ANALYTICS: true,
  DARK_MODE: true,
  BETA_FEATURES: false
};
```

---

## 🚀 Deployment

### Deploy Frontend (Vercel)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod

# Environment variables
# Set in Vercel dashboard: Settings → Environment Variables
```

### Deploy Backend (Railway)

```bash
# Install Railway CLI
npm i -g @railway/cli

# Login
railway login

# Initialize
railway init

# Deploy
railway up

# View logs
railway logs
```

### Deploy Database (Supabase)

```bash
# Create project on supabase.com
# Run migrations
supabase migration up

# Set up edge functions
supabase functions deploy

# Enable backups & monitoring
# Done in Supabase dashboard
```

### Full Deployment Guide

See [DEPLOYMENT.md](./docs/DEPLOYMENT.md) for detailed instructions including:
- CI/CD setup with GitHub Actions
- Environment management
- Database migrations in production
- Monitoring & logging setup
- Scaling strategies

---

## 🤝 Contributing

We love contributions! Here's how:

### Fork & Clone
```bash
git clone https://github.com/yourusername/flowtrip.git
cd flowtrip
git checkout -b feature/your-feature
```

### Make Changes
```bash
# Follow code style
npm run lint:fix

# Run tests
npm test

# Commit with clear message
git commit -m "feat: add awesome feature"
```

### Push & Create PR
```bash
git push origin feature/your-feature
# Create pull request on GitHub
```

### Code Style
- Use ESLint configuration
- Follow Prettier formatting
- Write JSDoc comments
- Add tests for new features

### Commit Messages
```
feat:   new feature
fix:    bug fix
docs:   documentation
style:  formatting
refactor: code restructuring
test:   adding tests
chore:  maintenance tasks
```

---



**Made with ❤️ by the Atharv Kulkarni**

*Last Updated: April 2024*
