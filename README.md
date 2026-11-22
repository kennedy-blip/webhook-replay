# WebhookReplay

Webhook delivery inspector, HMAC signature verifier, and safe replay console.

## Stack
- Vite + React + TypeScript
- Tailwind CSS v4
- Vercel Serverless Functions (`/api`)

## Development

```bash
npm install
npm run dev
```

For local API routes, use `vercel dev`. The frontend includes a graceful demo fallback when the API is unavailable.

## Deploy
Import this repository into Vercel. Use the repository root as the project root and the default Vite build command (`npm run build`).

> Demo note: the included in-memory event store is suitable for previews and demos. Serverless instances do not share memory and may reset; use a persistent database/queue for production workloads.