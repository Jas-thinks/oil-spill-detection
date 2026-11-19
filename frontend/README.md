# VesselWatch Dashboard

Next.js (App Router, TypeScript) monitoring UI for the VesselWatch oil-spill detection system.

## Pages

| Route | Description |
|---|---|
| `/` | Dashboard overview: key statistics and live predictions |
| `/map` | Leaflet map of incidents and vessel positions |
| `/incidents` | Incident table with SAR validation status |
| `/vessels` | Per-vessel statistics and history |
| `/analytics` | Aggregated analytics and charts |
| `/system-health` | Pipeline / infrastructure health |
| `/settings` | Application settings |

## Getting started

```bash
cd frontend
npm install
npm run dev        # http://localhost:3000
```

The UI talks to the FastAPI backend (see [`../backend`](../backend/README.md)), which must be running on port 8000. Real-time predictions are streamed over WebSocket.

## Scripts

| Command | Purpose |
|---|---|
| `npm run dev` | Start the dev server |
| `npm run build` | Production build |
| `npm run start` | Serve the production build |
| `npm run lint` | Run ESLint |
