# Himanshu Singh (Hunny Sins) - Futuristic 3D Portfolio

## Overview

This is a modern, futuristic 3D portfolio website for Himanshu Singh (aka Hunny Sins), a multi-dimensional creator specializing in AI, graphics, video editing, and digital arts. The application features an immersive 3D environment with cyberpunk aesthetics, showcasing various creative works and skills through interactive sections.

## System Architecture

### Frontend Architecture
- **React 18** with TypeScript for the user interface
- **Three.js** with React Three Fiber for 3D graphics and animations
- **Tailwind CSS** for styling with custom neon/cyberpunk theme
- **Radix UI** components for accessible UI elements
- **Vite** for fast development and building
- **TanStack Query** for data fetching and state management

### Backend Architecture
- **Express.js** server with TypeScript
- **In-memory storage** for basic data operations (currently using MemStorage)
- **RESTful API** design with `/api` prefix
- **Session management** capabilities (connect-pg-simple for future PostgreSQL sessions)

### Database Layer
- **Drizzle ORM** configured for PostgreSQL
- **Neon Database** as the serverless PostgreSQL provider
- **Schema-first approach** with TypeScript type safety
- **Migration system** using Drizzle Kit

## Key Components

### 3D Environment
- **Scene.tsx**: Main 3D scene with lighting, camera, and controls
- **Avatar.tsx**: Animated character with multiple actions (walking, dancing, sitting, etc.)
- **ParticleSystem.tsx**: 5000+ particles creating ambient effects
- **FloatingElements.tsx**: Animated geometric shapes throughout the scene
- **RobotTransformation.tsx**: DNA-to-robot transformation animation

### Portfolio Sections
- **Hero**: Introduction with neon text effects and profile display
- **Skills**: Interactive skill categories with progress bars
- **GraphicDesign**: Portfolio showcase for design work
- **VideoEditing**: Video project galleries
- **AILab**: AI projects and experiments showcase
- **NFTs**: Digital art collections and blockchain integration
- **YouTube**: Video content categorization and metrics
- **Poetry**: Creative writing with full-text display
- **Contact**: Multi-channel communication interface

### UI Components
- **NeonText**: Customizable text with glow effects in multiple colors
- **LiquidCursor**: Interactive cursor with ripple effects
- **Navigation**: Futuristic navigation with section switching
- **ServiceCenter**: Modal interface for user interactions

## Data Flow

1. **Application State**: Zustand stores manage portfolio navigation and audio controls
2. **Component Communication**: Props and context for 3D scene interactions
3. **API Layer**: Express routes handle future database operations
4. **Client-Side Routing**: Section-based navigation without page refreshes
5. **Real-time Updates**: Three.js animation loop drives 3D scene updates

## External Dependencies

### Core Technologies
- **@neondatabase/serverless**: Serverless PostgreSQL connection
- **@react-three/fiber**: React renderer for Three.js
- **@react-three/drei**: Three.js helpers and components
- **@tanstack/react-query**: Data fetching and caching
- **drizzle-orm**: Type-safe database operations

### UI/UX Libraries
- **@radix-ui/react-***: Accessible component primitives
- **@fontsource/inter**: Typography system
- **tailwindcss**: Utility-first CSS framework
- **framer-motion**: Animation library (implicit through Three.js)

### Development Tools
- **vite**: Build tool and dev server
- **typescript**: Type safety across the stack
- **eslint**: Code linting
- **prettier**: Code formatting

## Deployment Strategy

### Build Process
1. **Client Build**: Vite compiles React app to `dist/public`
2. **Server Build**: ESBuild bundles server code to `dist/index.js`
3. **Asset Optimization**: 3D models, shaders, and media files are processed
4. **Static Files**: Served from the public directory

### Environment Configuration
- **Development**: Hot module replacement with Vite middleware
- **Production**: Optimized builds with tree-shaking and minification
- **Database**: Environment-based DATABASE_URL configuration

### Performance Optimizations
- **Code Splitting**: React lazy loading for sections
- **3D Optimization**: Geometry instancing and texture atlasing
- **Asset Loading**: Progressive loading of 3D models and textures
- **Caching**: Query client configuration for API responses

## Changelog

```
Changelog:
- July 04, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```