# Eats'Kale

Eats'Kale is an AI-powered nutrition tracking app built with React, Vite, TypeScript, Tailwind CSS, shadcn/ui, and Supabase. It helps users log meals, analyze nutritional content, track goals, review progress, and install the app as a PWA.

## Features

- Meal tracking with AI-assisted food analysis
- Dashboard views for calories, macros, and progress
- Personalized nutrition goals
- Meal history and recipe-related flows
- Supabase authentication and protected app routes
- PWA support through Vite
- Light and dark theme support

## Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui and Radix UI
- Supabase
- TanStack Query
- React Router
- Recharts

## Getting Started

### Prerequisites

- Node.js 18 or newer
- npm
- A Supabase project

### Installation

```bash
npm install
```

### Environment Variables

Create a `.env` file in the project root and provide your Supabase credentials:

```bash
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_publishable_key
```

### Run Locally

```bash
npm run dev
```

The app will be available at the local URL printed by Vite, usually `http://localhost:5173`.

## Available Scripts

```bash
npm run dev
npm run build
npm run build:dev
npm run lint
npm run preview
```

## Project Structure

```text
src/
  components/          Reusable app and UI components
  hooks/               Custom React hooks
  integrations/        Supabase client and generated types
  lib/                 Shared utilities
  pages/               Route-level screens
supabase/
  functions/           Supabase Edge Functions
  migrations/          Database migrations
```

## Supabase

This project includes Supabase migrations and an `analyze-meal` Edge Function. Apply migrations and deploy functions through the Supabase CLI when setting up a new backend environment.

## Build

```bash
npm run build
```

The production build output is generated in `dist/`.
