# Vitalitree Landing Page (VDEV-023)

A single static `index.html` file with no build step and no dependencies. The only external request loads Atkinson Hyperlegible from Google Fonts.

The app itself lives in [Vitalitree-App](https://github.com/SENG455-Vitalitree/Vitalitree-App). This history was moved here from that repo's `landing/` folder ([PR #46](https://github.com/SENG455-Vitalitree/Vitalitree-App/pull/46)).

The design tokens (colours, type, radius, spacing) come from the POC style guide (`Vitalitree-POC/Style Guide.pdf`). The phone mockups are rebuilt in HTML from the POC screens: `family.tsx`, `SeniorAppointmentCard.tsx` and the Visit Questions flow.

## Preview locally

```bash
open index.html
```

## Deploy

Any static host works. The site is the repo root, with no build step.

- **GitHub Pages**: in repo Settings → Pages, choose "Deploy from a branch", select `main` and `/ (root)`. The site is served at `https://seng455-vitalitree.github.io/Vitalitree-Landing/`.
- **Netlify / Vercel**: create a new site from this repo and leave the build command and output directory empty.

## Placeholders to fill (marked with a red `*` on the page)

Hover any `*` on the page to see what it needs.

| Where | What's needed | Owner / ticket |
| --- | --- | --- |
| Every "Try live demo" button | Hosted release-candidate URL. Set `DEMO_URL` in the `<script>` at the bottom of `index.html` | VDEV-024 |
| Demo video section | Fallback demo recording embed | VDEV-024 |
| Nav logo, favicon, og:image | Final logo and wordmark (currently a tree mark in a teal tile) | VBIZ-014 |
| Pricing: Free plan | Confirm that a free tier exists, and its limits | BMC |
| Pricing: Family plan | Confirm $8 CAD/mo (tested in M2 interviews), member and record limits, annual option, cancellation terms | BMC |
| Comparison table note | Confirm the portal comparison claims | VBIZ-014 |
| FAQ: data storage | Hosting provider, encryption details, "never sell your data" policy | Dev and BCOM |
| FAQ: integrations, launch | Planned integrations, launch date or waitlist link | Team |
| Support email, Privacy, Terms | Real contact address and policy pages | Team |
