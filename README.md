# Spatz - Fullstack Svelte Template

A comprehensive fullstack template built with SvelteKit, featuring authentication, database integration, AI chatbots, and modern web technologies.

## Features

- **SvelteKit** - Modern fullstack web framework
- **PocketBase** - Backend with authentication and database
- **OpenAI Integration** - AI chatbot functionality
- **TailwindCSS** - Utility-first CSS framework
- **DaisyUI** - Component library for Tailwind
- **Zod** - Schema validation
- **TypeScript** - Type-safe development

## Tech Stack

- **SvelteKit** - Modern fullstack web framework
- **PocketBase** - Backend with authentication and database
- **OpenAI** - AI chatbot functionality
- **TailwindCSS** - Utility-first CSS framework
- **DaisyUI** - Component library
- **Zod** - Schema validation
- **TypeScript** - Type-safe development

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- PocketBase (download from pocketbase.io)
- pnpm package manager

### Installation

1. **PocketBase Setup:**
```bash
# Download and extract PocketBase
# Start PocketBase server
./pocketbase serve --http="0.0.0.0:8090"
```

2. **Client Setup:**
```bash
git clone <repository-url>
cd spatz
pnpm install
cp .env.example .env.local
# Edit .env.local with your configuration
pnpm run dev
```

3. Access the application at `http://localhost:5173`

### Environment Variables

Create a `.env.local` file with:
```env
PUBLIC_POCKETBASE_URL=http://localhost:8090
# Add other required environment variables
```

## Development

### Project Structure

```
/src
├── /lib
│   └── app.d.ts (global types)
├── /assets
│   └── /images
├── /components
├── /stores (global state)
├── /routes
│   ├── /guestbook
│   ├── /ai (nested routes)
│   │   ├── /a
│   │   ├── /b
│   │   └── /c
│   ├── /api
│   │   ├── /repoData (fetch github repository stars)
│   │   ├── /chat (OpenAI streaming API)
│   │__ /auth (Pocketbase auth)
│   │   ├── /login
│   │   ├── /register
│   │   ├── /logout
│   │   └── /reset-password
│   └── /my (user-specific routes)
│       ├── /account
│       ├── /profile
│       └── /settings
/pocketbase
├── pb_schema.json
/static
└── /docs (general documentation)
```

## Development

### Project Structure

```
/src
├── /lib
│   └── app.d.ts (global types)
├── /assets
│   └── /images
├── /components
├── /stores (global state)
├── /routes
│   ├── /guestbook
│   ├── /ai (nested routes)
│   │   ├── /a
│   │   ├── /b
│   │   └── /c
│   ├── /api
│   │   ├── /repoData (fetch github repository stars)
│   │   ├── /chat (OpenAI streaming API)
│   │__ /auth (Pocketbase auth)
│   │   ├── /login
│   │   ├── /register
│   │   ├── /logout
│   │   └── /reset-password
│   └── /my (user-specific routes)
│       ├── /account
│       ├── /profile
│       └── /settings
/pocketbase
├── pb_schema.json
/static
└── /docs (general documentation)

```

## Deployment

The application can be deployed to Vercel, Netlify, or any other hosting platform that supports SvelteKit applications.

### Additional Features

- **Icons**: Provided by Iconify/Svelte with searchable icon library
- **Theming**: Pre-loaded DaisyUI themes with custom theme creation options
- **Animations**: GSAP-powered animations for smooth user interactions

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests to improve the template.
