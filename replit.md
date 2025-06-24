# Portfolio Website Project

## Overview

This is a full-stack portfolio website built for a developer named Alex Thompson. The application showcases a personal portfolio with sections for hero, about, skills, projects, and contact information. It features a modern React frontend with shadcn/ui components and an Express.js backend with a contact form submission system.

## System Architecture

The application follows a full-stack architecture with clear separation between client and server:

- **Frontend**: React with TypeScript, using Vite as the build tool
- **Backend**: Express.js server with TypeScript
- **Database**: PostgreSQL with Drizzle ORM (currently using in-memory storage as fallback)
- **Styling**: Tailwind CSS with shadcn/ui component library
- **Animations**: Framer Motion for smooth interactions

## Key Components

### Frontend Architecture
- **React SPA**: Single-page application using Wouter for client-side routing
- **Component Library**: shadcn/ui for consistent, accessible UI components
- **State Management**: React Query (@tanstack/react-query) for server state management
- **Form Handling**: React Hook Form with Zod validation
- **Styling**: Tailwind CSS with custom design system and CSS variables for theming

### Backend Architecture
- **Express Server**: RESTful API server with middleware for logging and error handling
- **Database Layer**: Drizzle ORM configured for PostgreSQL with type-safe queries
- **Storage Strategy**: Currently using in-memory storage (MemStorage class) with interface for easy database integration
- **API Endpoints**: 
  - `POST /api/contact` - Submit contact form
  - `GET /api/contacts` - Retrieve all contacts (admin functionality)

### Database Schema
- **Contacts Table**: Stores contact form submissions with fields for name, email, subject, message, and timestamp
- **Type Safety**: Drizzle-zod integration for runtime validation matching database schema

## Data Flow

1. **Contact Form Submission**:
   - User fills out contact form on frontend
   - Form validation using Zod schema (client-side)
   - API request to backend endpoint
   - Server validates data and stores in database/memory
   - Success/error response sent back to client
   - Toast notification displayed to user

2. **Portfolio Display**:
   - Static content rendered from component data
   - Smooth scrolling navigation between sections
   - Animated elements using Framer Motion with intersection observers

## External Dependencies

### Frontend Dependencies
- **React Ecosystem**: React 18, React DOM, React Hook Form
- **UI/UX**: shadcn/ui (Radix UI primitives), Framer Motion, Lucide icons
- **Styling**: Tailwind CSS, class-variance-authority, clsx
- **HTTP Client**: Native fetch API with React Query
- **Routing**: Wouter (lightweight React router)

### Backend Dependencies
- **Server**: Express.js with TypeScript support
- **Database**: Drizzle ORM, @neondatabase/serverless (for Neon PostgreSQL)
- **Validation**: Zod for schema validation
- **Development**: tsx for TypeScript execution, Vite for frontend bundling

### Development Tools
- **Build Tools**: Vite, esbuild for server bundling
- **TypeScript**: Full TypeScript support across frontend and backend
- **Database Tools**: Drizzle Kit for migrations and schema management

## Deployment Strategy

The application is configured for deployment on Replit with the following setup:

- **Environment**: Node.js 20 with PostgreSQL 16 support
- **Build Process**: Vite builds frontend assets, esbuild bundles server code
- **Production Server**: Serves static files and API endpoints from single Express server
- **Development**: Hot module replacement with Vite dev server proxy
- **Database**: Configured for PostgreSQL with environment variable for connection string

### Build Commands
- `npm run dev` - Development mode with hot reloading
- `npm run build` - Production build (frontend + backend)
- `npm run start` - Production server
- `npm run db:push` - Push database schema changes

## Recent Changes
- June 23, 2025: Complete portfolio website deployed with database integration
- June 23, 2025: Successfully pushed to GitHub repository
- June 23, 2025: All components working - contact form, project showcase, responsive design

## Changelog  
- June 23, 2025: Initial portfolio website setup with React, TypeScript, Express.js
- June 23, 2025: PostgreSQL database integration with Drizzle ORM
- June 23, 2025: Contact form with database storage functionality
- June 23, 2025: Complete documentation and GitHub setup guide created
- June 23, 2025: Project successfully pushed to GitHub

## User Preferences

Preferred communication style: Simple, everyday language.