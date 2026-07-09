# LakelandFinds — Local Business Directory for Lakeland, FL

A Yelp-style local business directory built with Next.js, focused on Lakeland, Florida. Residents browse and discover local businesses by category; business data is seeded and enriched through automated pipelines.

## Features

- Business listings organized by category for the Lakeland market
- Search and browse experience built on the Next.js App Router
- Database-backed listings with automated seeding (`seed.ts`) and standalone data enrichment (`enrich-standalone.ts`)
- Container-ready deployment (`Dockerfile` included)

## Tech Stack

- **Framework:** Next.js (App Router) + TypeScript
- **Styling:** Tailwind CSS
- **Database:** Drizzle ORM (`drizzle.config.ts`)
- **Infra:** Docker, environment-based config (`.env.example`)

## Project Structure

```
app/          — routes and pages (Next.js App Router)
components/   — shared UI components
hooks/        — custom React hooks
lib/          — utilities and data access
scripts/      — operational scripts
seed.ts       — database seeding
enrich-standalone.ts — business data enrichment pipeline
```

## Getting Started

```bash
cp .env.example .env   # fill in your database credentials
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## About

Built by World Unities LLC as part of a portfolio of local-market web platforms for Central Florida. See more at [github.com/danieljames-dev](https://github.com/danieljames-dev).
