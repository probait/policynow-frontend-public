# PolicyNow Canada (Public Frontend – Hackathon Edition)

**Website:** https://policynow.ca  
**Hackathon:** Vancouver BC-AI – Round 3  
**Status:** This is a *sanitized* public repository for judging. Our private repo contains backend, infrastructure, admin, and deployment details for security reasons.

## What is PolicyNow?
PolicyNow is a civic technology platform that collects and publishes Canadian public perspectives on AI, blockchain, and other emerging technologies, producing a living civic dataset for policymakers, researchers, and the public.

### Voices Across Canada
We transform raw submissions into short, readable “voice blurbs,” then map them geographically (currently across BC) on the Dataset page. The map includes filterable sentiment clusters (positive, neutral, negative, unknown) and will expand nationwide.

## Core features (visible in the live site)
- Public submission form with location and topic tags
- Filterable community feed of voice blurbs
- Dataset map with sentiment clustering (CARTO / OSM tiles)
- Contributor recognition (profiles, features, fellowships – in progress)
- Newsletter integration

## Tech stack (public portion)
- Frontend: Next.js / React
- Styling: Tailwind CSS
- Map: client-side rendering against public tiles
- Auth & API: *not included here* (private). This repo uses mocked endpoints for local dev.

## Run locally (frontend only)
```bash
npm install
cp .env.example .env.local
npm run dev
```
> Note: Endpoints are mocked. Replace `NEXT_PUBLIC_API_BASE_URL` with your own dev API to test writes.

## Repo hygiene
- No secrets are committed.
- Backend, DB schemas, and deployment files are excluded by design.
- See **SECURITY.md** for our policy, and **docs/submission_overview.md** for the hackathon narrative.

## License
MIT (see LICENSE)
