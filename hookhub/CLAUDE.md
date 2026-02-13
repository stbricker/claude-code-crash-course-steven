# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HookHub is a Next.js 16 application using the App Router architecture with React 19, TypeScript, and Tailwind CSS v4.

## Development Commands

```bash
# Start development server (localhost:3000)
npm run dev

# Build for production
npm run build

# Start production server
npm run start

# Run ESLint
npm run lint
```

## Architecture

### App Router Structure
- Uses Next.js App Router with the `app/` directory
- `app/layout.tsx`: Root layout with Geist font configuration and global CSS
- `app/page.tsx`: Home page component
- `app/globals.css`: Global Tailwind CSS styles

### TypeScript Configuration
- Strict mode enabled
- Path alias: `@/*` maps to project root
- Target: ES2017 with modern ESNext modules
- JSX set to `react-jsx` for React 19

### Styling
- Tailwind CSS v4 with PostCSS
- Uses `@tailwindcss/postcss` plugin
- Geist Sans and Geist Mono fonts loaded via `next/font/google`
- Supports dark mode via `dark:` class prefix

### ESLint
- Uses ESLint 9 flat config format (eslint.config.mjs)
- Configured with Next.js recommended rules (`eslint-config-next`)
- Ignores: `.next/`, `out/`, `build/`, `next-env.d.ts`

## Key Dependencies

- Next.js 16.1.6
- React 19.2.3
- TypeScript 5
- Tailwind CSS v4
- ESLint 9

## File Conventions

- Use `.tsx` for React components
- Use `.ts` for utility functions and non-component code
- Place static assets in `public/` directory
- Use TypeScript strict mode - all types must be properly defined
