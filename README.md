# Emergency Cleanings — State Location Landing Pages

State-level hoarding cleanup landing pages for [EmergencyCleanings.com](https://emergencycleanings.com).

## Pages

| Page | URL | Status |
|------|-----|--------|
| Florida Hoarding Cleanup | `/florida-hoarding-cleanup/` | Draft |
| Ohio Hoarding Cleanup | `/ohio-hoarding-cleanup/` | Draft |

## Structure

```
ec-location-pages/
├── vercel.json                        ← Vercel routing config
├── shared/
│   └── styles.css                     ← Brand tokens, shared components
├── florida-hoarding-cleanup/
│   └── index.html                     ← FL landing page
└── ohio-hoarding-cleanup/
    └── index.html                     ← OH landing page
```

## Brand Standards

All pages are built to EC Brand Voice Guidelines v2 (May 2026):
- Colors: `#0f1f38` (navy dark), `#234372` (navy), `#fef22e` (yellow CTA), `#2f64e7` (section labels)
- Font: Inter (Google Fonts)
- Voice: The Ally archetype — direct, warm, competent
- QA score: 9.5/10 (both pages)

## Deployment

Deployed to Vercel. Each push to `main` triggers an automatic redeploy.

## Adding New States

1. Copy an existing state folder (e.g., `florida-hoarding-cleanup/`)
2. Rename to `[state]-hoarding-cleanup/`
3. Update: state name, city grid, testimonials, state-specific feature (6th feature card), FAQ if needed
4. Add route entry to `vercel.json`
5. Push — Vercel auto-deploys
