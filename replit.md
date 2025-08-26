# El Planner Anti-Fracaso

## Overview

El Planner Anti-Fracaso is a comprehensive productivity planning application designed to help users achieve their goals through structured daily, weekly, and monthly planning. The app features an AI-powered "Guru" that provides motivational phrases and guidance, along with tools for financial tracking, manifestation practices, and progress monitoring. Built with a freemium model, it offers basic functionality for free users and premium features for subscribers.

The application is designed around a Spanish-speaking audience and uses a sarcastic yet motivational "Guru" personality to engage users and keep them accountable to their goals.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript, built using Vite
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query (React Query) for server state management
- **UI Framework**: Radix UI components with shadcn/ui design system
- **Styling**: Tailwind CSS with custom color scheme (black and orange theme)
- **Form Handling**: React Hook Form with Zod validation

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Authentication**: Session-based authentication with PIN security
- **API Design**: RESTful API endpoints with structured error handling
- **File Organization**: Monorepo structure with shared schema between client and server

### Data Storage Solutions
- **Database**: PostgreSQL using Neon serverless database
- **Session Storage**: Express sessions with connect-pg-simple for PostgreSQL session store
- **Schema Management**: Drizzle Kit for database migrations and schema management
- **Data Validation**: Zod schemas for runtime type checking and validation

### Authentication and Authorization
- **Security Model**: PIN-based authentication instead of traditional username/password
- **Session Management**: Server-side sessions with secure HTTP-only cookies
- **Access Control**: Role-based access with freemium tier restrictions
- **Premium Features**: Subscription-based feature gating for advanced functionality

### Core Application Features
- **Daily Planning**: Task management, time blocking, mood tracking, and gratitude journaling
- **Weekly Planning**: Goal setting, mini-objectives, achievements tracking, and energy level monitoring
- **Monthly Goals**: Main goal setting, sub-goals, habit tracking, and life balance wheel
- **Financial Management**: Income/expense tracking, savings goals, and AI-generated financial advice
- **Manifestation Tools**: Scripting area, 21-day habit tracker, and visualization boards
- **Reflection System**: Morning and evening guided reflection prompts
- **Progress Analytics**: Comprehensive progress tracking across all planning areas

### AI Integration Architecture
- **AI Provider**: OpenAI GPT integration for dynamic content generation
- **Guru Personality**: Custom prompts for sarcastic yet motivational coaching phrases
- **Content Types**: Daily motivational phrases, financial advice, and progress-based feedback
- **Personalization**: Context-aware AI responses based on user progress and behavior

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL hosting with connection pooling
- **Database Driver**: @neondatabase/serverless for optimized serverless connections

### AI and Machine Learning
- **OpenAI API**: GPT models for generating personalized motivational content and advice
- **Custom Prompting**: Specialized prompts for maintaining consistent "Guru" personality

### UI and Design System
- **Radix UI**: Comprehensive set of accessible React components
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Lucide React**: Icon library for consistent iconography
- **Google Fonts**: Custom font loading for typography

### Development and Build Tools
- **Vite**: Fast build tool and development server
- **TypeScript**: Type safety across the entire application
- **ESBuild**: Fast JavaScript bundler for production builds
- **PostCSS**: CSS processing with autoprefixer

### Validation and Forms
- **Zod**: Runtime type validation and schema definition
- **React Hook Form**: Performant form handling with minimal re-renders
- **Drizzle Zod**: Integration between Drizzle ORM and Zod schemas

### Session and State Management
- **Express Session**: Server-side session management
- **TanStack Query**: Powerful data fetching and caching for React
- **Connect PG Simple**: PostgreSQL session store for Express

### Utility Libraries
- **Date-fns**: Date manipulation and formatting
- **Bcrypt**: Password hashing for PIN security
- **Class Variance Authority**: Utility for creating variant-based component APIs
- **CLSX**: Conditional class name utility