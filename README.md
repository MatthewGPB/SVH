# South Village Development — Investor Site

Single-page Astro site for South Village Development LLC (near south side Indianapolis).

## Stack
- Astro 5 (static output) → deploys to Vercel with zero config
- Photography in `public/images/` (pre-optimized JPEGs)
- One page: `src/pages/index.astro`; global styles in `src/layouts/Base.astro`

## Local dev
```
npm install
npm run dev        # http://localhost:4321
npm run build      # outputs to dist/
```

## Deploy (GitHub → Vercel)
1. Create a GitHub repo and push this folder.
2. In Vercel: **Add New Project → Import** the repo. Vercel auto-detects Astro (build `astro build`, output `dist/`). No adapter or env vars needed.
3. Add the custom domain in Vercel → Project → Settings → Domains.

## Before launch — placeholders to replace
- `contactEmail` in `src/pages/index.astro` (currently invest@southvillagedev.com)
- Cruz and Matthew: full names, bios, headshots (drop headshots in `public/images/`, swap the `.ph` initial divs for `<img>` like Gabe's)
- Confirm the wordmark: "South Village" vs "South Village Homes" vs "South Village Development"
- `site` URL in `astro.config.mjs` once the domain is final
