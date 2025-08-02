# SmartCalc Tool

## Overview

SmartCalc is a comprehensive web application featuring seven different types of calculators in one unified interface. The application provides simple, loan, pregnancy, percentage, age, area, and scientific calculators with a modern, responsive design supporting both light and dark themes. Built as a full-stack application with React frontend and Express backend, it includes calculation history tracking and a clean, intuitive user interface.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript using Vite as the build tool
- **UI Library**: Shadcn/ui components built on top of Radix UI primitives
- **Styling**: Tailwind CSS with CSS variables for theming
- **State Management**: React hooks for local state, TanStack React Query for server state
- **Routing**: Wouter for lightweight client-side routing
- **Theme System**: Custom theme hook with localStorage persistence and system preference detection

### Component Structure
- **Calculator Components**: Seven specialized calculator components (Simple, Loan, Pregnancy, Percentage, Age, Area, Scientific)
- **Shared Components**: History panel, theme toggle, and reusable UI components
- **Layout**: Tab-based interface for switching between calculator types
- **History Management**: Per-calculator history tracking with localStorage persistence

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Development Setup**: Custom Vite integration for development with hot module replacement
- **Storage Interface**: Abstracted storage layer with in-memory implementation (ready for database integration)
- **API Structure**: RESTful endpoints with /api prefix
- **Error Handling**: Centralized error handling middleware

### Database Schema
- **ORM**: Drizzle ORM configured for PostgreSQL
- **Schema**: User table with UUID primary keys, username, and password fields
- **Migrations**: Drizzle Kit for schema management and migrations
- **Connection**: Configured for Neon Database serverless PostgreSQL

### Styling and Theming
- **Design System**: Shadcn/ui "new-york" style variant
- **Color Scheme**: CSS custom properties for light/dark theme support
- **Typography**: Inter font family for consistent typography
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints

### Development Tools
- **Build System**: Vite for frontend, esbuild for backend production builds
- **TypeScript**: Strict configuration with path mapping for clean imports
- **Code Quality**: ESM modules throughout the application
- **Development Experience**: Hot reload, error overlays, and development banners

## External Dependencies

### Core Frontend Libraries
- **React Ecosystem**: React 18, React DOM, React Hook Form with Zod validation
- **UI Components**: Radix UI primitives for accessible component foundations
- **Styling**: Tailwind CSS, class-variance-authority for component variants
- **State Management**: TanStack React Query for server state management
- **Utilities**: date-fns for date manipulation, clsx for conditional styling

### Backend Dependencies  
- **Server Framework**: Express.js with TypeScript support
- **Database**: Drizzle ORM with PostgreSQL dialect, Neon Database serverless driver
- **Session Management**: connect-pg-simple for PostgreSQL session storage
- **Development**: tsx for TypeScript execution, Vite for development server

### Build and Development Tools
- **Build Tools**: Vite, esbuild, PostCSS with Autoprefixer
- **TypeScript**: Full TypeScript support with strict configuration
- **Replit Integration**: Replit-specific plugins for development environment
- **UI Development**: Embla Carousel for carousel components, Vaul for drawer components

### Database and Storage
- **Database**: PostgreSQL via Neon Database serverless
- **ORM**: Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema updates
- **Local Storage**: Browser localStorage for calculator history and theme preferences