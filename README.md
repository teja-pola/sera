# Sera Ai - Agentic AI Platform for Brands and Creators

Sera Ai is a platform that revolutionizes the way brands discover and collaborate with content creators. Built with modern web technologies, it provides an intelligent matching system that connects brands with the right creators based on AI-powered analytics and compatibility scoring.

## What Problem Does Sera Ai Solve?

The creator economy is booming, but finding the right brand-creator partnerships remains a significant challenge:

- **For Brands**: Discovering creators who align with brand values, target audience, and campaign goals is time-consuming and often relies on manual research
- **For Creators**: Finding relevant brand collaboration opportunities requires extensive networking and outreach efforts
- **Inefficient Matching**: Traditional methods don't leverage data-driven insights to ensure successful partnerships

Sera Ai solves these problems by:

- **AI-Powered Matching**: Uses advanced algorithms to match brands with creators based on audience demographics, engagement metrics, content style, and brand alignment
- **Streamlined Discovery**: Provides brands with curated creator recommendations and gives creators visibility to relevant opportunities
- **Data-Driven Decisions**: Offers comprehensive analytics and insights to help both parties make informed collaboration decisions
- **Automated Workflows**: Reduces manual work through intelligent automation of matching, application processes, and communication

## What Sera Ai Does

Sera Ai is a full-stack platform that includes:

### For Brands
- **Creator Discovery**: Browse and search through a curated database of content creators
- **AI Matching**: Receive intelligent recommendations based on campaign requirements
- **Analytics Dashboard**: Track campaign performance and creator metrics
- **Application Management**: Review and manage creator applications efficiently

### For Creators
- **Profile Analytics**: Get AI-powered insights into your social media performance
- **Brand Discovery**: Find relevant brand collaboration opportunities
- **Dynamic Pricing**: Generate rate cards based on your engagement metrics
- **Application System**: Apply to brand campaigns with ease

## Architecture

- **Frontend**: React.js with Tailwind CSS - Modern, responsive user interface
- **Backend**: Node.js with Express and MongoDB - Scalable REST API
- **AI Integration**: Google Generative AI (Gemini) for profile analysis and matching
- **Authentication**: JWT-based with email verification and Google OAuth

## Quick Start

### Prerequisites

Make sure you have the following installed:
- Node.js (v16 or higher)
- MongoDB (running locally or connection string)
- npm or yarn package manager

### Backend Setup

1. Navigate to backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env` (if available) or create a `.env` file
   - Configure the following variables:
     ```env
     NODE_ENV=development
     PORT=8000
     MONGO_URL=mongodb://localhost:27017
     DB_NAME=sera_ai_db
     JWT_SECRET=your_jwt_secret_key
     GEMINI_API_KEY=your_gemini_api_key
     FRONTEND_URL=http://localhost:3000
     CORS_ORIGINS=http://localhost:3000
     ```

4. Start development server:
   ```bash
   npm run dev
   ```

   The API will be available at `http://localhost:8000`

### Frontend Setup

1. Navigate to frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables (if needed):
   - Create a `.env` file with:
     ```env
     REACT_APP_API_URL=http://localhost:8000
     ```

4. Start development server:
   ```bash
   npm run dev
   ```

   The app will be available at `http://localhost:3000`

## Tech Stack

### Backend
- Node.js & Express.js
- MongoDB with Mongoose
- JWT Authentication
- Google Generative AI (Gemini)
- bcrypt for password hashing
- Winston for logging
- Helmet for security

### Frontend
- React.js
- Tailwind CSS
- React Router
- Axios for API calls

## Project Structure

```
sera-ai/
├── backend/          # Node.js Express API
│   ├── models/       # MongoDB schemas (User, Session)
│   ├── routes/       # API endpoints (auth, health)
│   ├── middleware/   # Auth, validation, error handling, security
│   ├── utils/        # Helper utilities (JWT, logger, email, etc.)
│   ├── migrations/  # Database migrations
│   └── server.js     # Main server file
├── frontend/         # React application
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/      # Page components
│   │   └── utils/       # Frontend utilities
│   └── public/          # Static assets
└── README.md
```

## Features

- **User Authentication**: Secure signup, login, email verification, and Google OAuth
- **Session Management**: JWT-based session handling with refresh tokens
- **Health Monitoring**: Comprehensive health check endpoints
- **Security**: Rate limiting, input validation, XSS protection, MongoDB injection prevention
- **Error Handling**: Structured error responses with logging
- **Email System**: Automated verification and notification emails


## Acknowledgments

- Built with modern web technologies
- Powered by Google Generative AI (Gemini)
