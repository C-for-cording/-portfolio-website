# Portfolio Website

A modern, responsive portfolio website built with React, TypeScript, and Express.js.

## Features

- 🎨 Modern and responsive design
- 📱 Mobile-first approach
- 🎯 Smooth scrolling navigation
- 📊 Interactive skills section
- 🎪 Project showcase with filtering
- 📬 Contact form with database integration
- ⚡ Fast performance with Vite
- 🗄️ PostgreSQL database

## Tech Stack

### Frontend
- React 18 with TypeScript
- Tailwind CSS for styling
- Framer Motion for animations
- React Hook Form with Zod validation
- TanStack Query for state management
- shadcn/ui components

### Backend
- Express.js with TypeScript
- PostgreSQL with Drizzle ORM
- Neon database integration
- RESTful API endpoints

## Getting Started

1. Clone the repository
```bash
git clone <repository-url>
cd portfolio-website
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
# Database connection will be automatically configured on Replit
```

4. Push database schema
```bash
npm run db:push
```

5. Start the development server
```bash
npm run dev
```

## Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── lib/           # Utility functions
│   │   └── hooks/         # Custom hooks
├── server/                # Backend Express server
│   ├── db.ts             # Database connection
│   ├── storage.ts        # Data access layer
│   └── routes.ts         # API routes
├── shared/               # Shared types and schemas
└── components.json       # shadcn/ui configuration
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run db:push` - Push database schema changes

## Deployment

This project is configured for deployment on Replit with automatic database provisioning.

## Contact

For any questions or suggestions, please use the contact form on the website.