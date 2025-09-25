# Overview

This is a full-stack order management system built with React/TypeScript frontend and Express.js backend. The application allows users to submit product orders through a web form, with features including product catalog management, dynamic pricing with tier calculations, order validation, and external integration with Google Apps Script for order processing. The system uses PostgreSQL for data persistence and shadcn/ui for the user interface components.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript and Vite for build tooling
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: React Hook Form for form state and validation with Zod schemas
- **Data Fetching**: TanStack Query (React Query) for server state management and caching
- **UI Components**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with CSS custom properties for theming
- **Type Safety**: Full TypeScript coverage with strict mode enabled

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema management
- **API Design**: RESTful endpoints with JSON responses
- **Error Handling**: Centralized error middleware with structured error responses
- **Environment**: Development and production configurations with Vite integration

## Data Storage Solutions
- **Primary Database**: PostgreSQL hosted on Neon Database
- **ORM**: Drizzle ORM for type-safe database queries and migrations
- **Schema**: Shared TypeScript schemas between frontend and backend using Zod
- **Tables**: Orders and Products tables with JSONB fields for flexible data structures
- **Validation**: Runtime validation using Zod schemas derived from database schema

## Authentication and Authorization
- **Current State**: No authentication system implemented
- **Session Management**: Express session configuration present but not actively used
- **Security**: Basic CORS and request logging middleware

## External Dependencies
- **Database**: Neon Database (PostgreSQL-compatible serverless database)
- **Google Apps Script**: External integration for order processing and notifications
- **UI Components**: Radix UI primitives for accessible component foundation
- **Build Tools**: Vite for frontend bundling and development server
- **Styling**: Tailwind CSS for utility-first styling approach
- **Fonts**: Google Fonts integration (Inter, DM Sans, Fira Code, Geist Mono)
- **Development**: Replit-specific plugins for development environment integration