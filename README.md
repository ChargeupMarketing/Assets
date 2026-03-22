# Conversation Studio

LinkedIn-first conversation intelligence and engagement copilot built with Next.js, Supabase, and OpenAI-ready API routes.

## What is included
- Dashboard pages for live monitor, trends, people finder, inbox, review, and settings
- Mock API routes so the app runs immediately
- Supabase SQL schema for core entities
- Environment template
- Project structure ready for connector work and AI wiring

## Quick start
1. Install dependencies
   npm install
2. Copy environment file
   cp .env.example .env.local
3. Add your Supabase keys
4. Run the app
   npm run dev

## Deploy on Vercel
1. Push this folder to GitHub
2. Import the repo into Vercel
3. Add environment variables from `.env.example`
4. Deploy

## Create the database
1. Open Supabase SQL editor
2. Paste `supabase/schema.sql`
3. Run the migration

## What to replace next
- Replace mock discovery routes with real connector ingestion
- Add Supabase reads and writes into the route handlers
- Add OpenAI calls in the AI routes
- Add auth and workspace-aware row level security

## Suggested hosting
- Frontend/API: Vercel
- Database/Auth/Realtime: Supabase

## Important note
This scaffold is intentionally safe to host right away. Direct LinkedIn reply/post actions should remain feature-flagged until your connector and permissions are confirmed.
