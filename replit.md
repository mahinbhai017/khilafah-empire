# Khilafah Empire - Entrepreneurship Platform

## Overview

This is a full-stack web application for "Khilafah Empire," an Islamic entrepreneurship platform founded by MaHiN SHeikH. The application provides ready-to-launch business packages for Muslim entrepreneurs, combining modern business strategies with Islamic principles. The platform features a contact system for potential clients to inquire about business opportunities.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite for development and building
- **Routing**: Wouter for client-side routing
- **Styling**: Tailwind CSS with shadcn/ui component library
- **UI Theme**: Dark theme with Islamic-inspired color scheme (emerald green and gold accents)
- **State Management**: TanStack Query (React Query) for server state management
- **Form Handling**: React Hook Form with Zod validation
- **Animations**: Framer Motion for smooth transitions and interactive elements

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Language**: TypeScript with ES modules
- **API Style**: RESTful API endpoints
- **Development**: Hot reload using tsx for development
- **Production**: Compiled using esbuild for optimal performance

### Data Storage Solutions
- **Database**: PostgreSQL configured for production deployment
- **ORM**: Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Development Storage**: In-memory storage implementation for development/testing
- **Database Provider**: Neon Database (serverless PostgreSQL)

## Key Components

### Database Schema
The application defines two main entities:
- **Users**: Authentication system with username/password
- **Contacts**: Contact form submissions with business interests and timestamps

### API Endpoints
- `POST /api/contact`: Submit contact form with validation
- `GET /api/contacts`: Retrieve all contact submissions (admin functionality)

### Frontend Pages
- **Home**: Landing page with Islamic greetings and call-to-action
- **About**: Information about MaHiN SHeikH and his mission
- **Services**: Three main entrepreneurship packages offered
- **Gallery**: Success stories and visual content
- **Contact**: Contact form for business inquiries

### Interactive Features
- **Audio Player**: Quran recitation with volume control
- **Chatbot**: Customer service interface with Islamic greetings
- **Floating Assistant**: Draggable help interface
- **Horse Intro**: Animated introduction sequence
- **Mobile Responsive**: Fully responsive design with mobile navigation

## Data Flow

1. **User Interaction**: Users navigate through pages and interact with forms
2. **Form Submission**: Contact forms are validated client-side using Zod schemas
3. **API Communication**: Forms submit to REST endpoints with proper error handling
4. **Data Persistence**: Contact submissions are stored in PostgreSQL database
5. **Real-time Updates**: TanStack Query manages cache invalidation and updates
6. **Response Handling**: Success/error messages displayed via toast notifications

## External Dependencies

### UI and Styling
- Radix UI primitives for accessible components
- Tailwind CSS for utility-first styling
- Font Awesome for icons
- Google Fonts (Inter and Amiri for Arabic text)

### Database and Backend
- Neon Database for serverless PostgreSQL
- Drizzle ORM for database operations
- Connect-pg-simple for session management

### Development Tools
- Vite for fast development and building
- TypeScript for type safety
- ESLint and Prettier (implied by project structure)

## Deployment Strategy

### Development Environment
- Replit platform with PostgreSQL module
- Hot reload development server on port 5000
- Vite development server with middleware integration

### Production Build
- Frontend: Vite builds static assets to `dist/public`
- Backend: esbuild compiles server code to `dist/index.js`
- Database: Drizzle migrations manage schema changes

### Environment Configuration
- Database connection via `DATABASE_URL` environment variable
- Development vs production modes handled automatically
- Static file serving for production deployments

## Changelog

Changelog:
- June 20, 2025. Initial setup
- June 20, 2025. Added Nathan Gao-inspired flowing organic shapes with animated text paths and Islamic geometric elements to home page

## User Preferences

Preferred communication style: Simple, everyday language.