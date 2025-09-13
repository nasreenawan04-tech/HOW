# Frontend Tools App - Replit Project Documentation

## Overview
This is a comprehensive frontend application featuring a collection of useful tools including calculators, converters, and generators. The app provides finance tools, health calculators, text utilities, and more in a modern React-based interface.

**Current State:** Fully functional and running on Replit with proper development server configuration.

## Recent Changes
- **September 13, 2025:** Initial Replit environment setup completed
  - Installed all dependencies via npm
  - Configured development workflow on port 5000
  - Verified application functionality and accessibility
  - Set up proper Replit integration with Vite configuration

## Project Architecture

### Frontend Stack
- **Framework:** React 18 with TypeScript
- **Build Tool:** Vite 5.4.19 with hot module replacement
- **Routing:** Wouter for client-side routing
- **UI Library:** Radix UI components with Tailwind CSS
- **State Management:** TanStack React Query for server state
- **Styling:** Tailwind CSS with custom component system
- **Icons:** Lucide React icons

### Key Features
- **Tool Categories:**
  - Finance calculators (loan, mortgage, EMI, compound interest, etc.)
  - Health calculators (BMI, BMR, calorie, ideal weight, etc.)
  - Text tools (word counter, case converter, password generator, etc.)
  - QR code generation and scanning
  - Currency and cryptocurrency conversion

- **User Experience:**
  - Responsive design with mobile-first approach
  - Dark/light theme support via next-themes
  - Lazy loading for performance optimization
  - Favorites and recently used tools tracking
  - Search functionality with Fuse.js

### Project Structure
```
client/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── ui/             # Base UI components (buttons, cards, etc.)
│   │   └── [other components]
│   ├── pages/              # Page components for each tool
│   ├── hooks/              # Custom React hooks
│   ├── lib/                # Utility libraries and configurations
│   ├── data/               # Static data (tools configuration)
│   ├── App.tsx             # Main application router
│   └── main.tsx            # Application entry point
├── public/                 # Static assets
└── index.html              # HTML template
```

### Configuration Files
- **vite.config.ts:** Vite configuration with Replit-specific settings
- **tailwind.config.ts:** Tailwind CSS configuration
- **tsconfig.json:** TypeScript configuration
- **package.json:** Dependencies and scripts

## Development Setup

### Running the Application
The application is configured to run on Replit with the following workflow:
- **Command:** `npm run dev`
- **Port:** 5000 (properly configured for Replit proxy)
- **Host:** 0.0.0.0 (allows external access through Replit's proxy)

### Build System
- **Development:** Vite dev server with HMR
- **Production:** Vite build system generates optimized static files
- **Scripts:**
  - `npm run dev` - Start development server
  - `npm run build` - Build for production
  - `npm run preview` - Preview production build

### Replit Integration
- Configured with Replit-specific Vite plugins:
  - `@replit/vite-plugin-runtime-error-modal` for error overlay
  - `@replit/vite-plugin-cartographer` for code navigation
- HMR clientPort set to 443 for Replit's proxy system
- Proper host configuration (0.0.0.0) for external access

## User Preferences
- No specific user preferences documented yet

## Dependencies
### Core Dependencies
- React 18.3.1 with React DOM
- TypeScript 5.6.3
- Vite 5.4.19 with React plugin
- Wouter 3.3.5 for routing
- TanStack React Query 5.60.5

### UI & Styling
- Tailwind CSS 3.4.17 with various plugins
- Radix UI component library (extensive collection)
- Lucide React icons
- Framer Motion for animations

### Utilities
- Zod for schema validation
- React Hook Form with resolvers
- Date-fns for date handling
- Axios for HTTP requests
- QR code libraries (qrcode, qr-scanner)
- Fuse.js for fuzzy search

## Technical Notes
- The application uses lazy loading extensively for performance
- All major routes are code-split for optimal loading
- Proper TypeScript configuration with strict mode
- Modern CSS with Tailwind utility classes
- Responsive design principles throughout

## Status
✅ **Ready for use** - Application is fully functional and properly configured for the Replit environment.