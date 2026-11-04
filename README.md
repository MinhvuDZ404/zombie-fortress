# DEAD ZONE — Sinh Tồn Trong Đại Dịch Zombie

A top-down zombie survival shooter built with Next.js, React, TypeScript, and a custom Canvas 2D game engine.

## Game features

- Wave-based zombie survival combat.
- Six weapons, multiple zombie archetypes, elite variants, and boss encounters.
- Roguelite upgrade choices between waves.
- Desktop keyboard/mouse and mobile touch controls.
- Local settings and a leaderboard API.

## Technology

- Next.js 16, React 19, TypeScript
- Custom Canvas 2D game engine
- Prisma ORM with SQLite
- Tailwind CSS

## Local development

Requirements: Bun (recommended) or Node.js 20+.

```bash
bun install
bun run dev
```

Open http://localhost:3000.

The leaderboard API uses Prisma and requires a valid `DATABASE_URL`. Configure it in a local `.env` file and initialize the database using the Prisma schema before using leaderboard features.

## Deployment

The full app includes a Next.js API route and a Prisma/SQLite backend. GitHub Pages only serves static files and cannot run this backend. To publish the complete playable game, deploy the Next.js app to a Node.js-capable host and configure a persistent production database.

## Repository hygiene

Never commit `.env` files, credentials, local database files, runtime logs, test screenshots, or machine-specific state.
