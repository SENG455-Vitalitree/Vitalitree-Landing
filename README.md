# Vitalitree Landing Page (VDEV-023)

A single static `index.html` file with no build step and no dependencies. The only external request loads Atkinson Hyperlegible from Google Fonts.

The design tokens (colours, type, radius, spacing) come from the POC style guide (`Vitalitree-POC/Style Guide.pdf`). The phone mockups are rebuilt in HTML from the POC screens: `family.tsx`, `SeniorAppointmentCard.tsx` and the Visit Questions flow.

## Preview locally

```bash
open landing/index.html
```

## Deploy

Any static host works. Point it at the `landing/` folder:

- **Netlify / Vercel**: create a new site from this repo, set the base/output directory to `landing`, and leave the build command empty.
- **GitHub Pages**: the org repos are private, so Pages needs a paid plan or a separate public repo that holds just `landing/`.

## Placeholders to fill (marked with a red `*` on the page)

Hover any `*` on the page to see what it needs.

| Where | What's needed | Owner / ticket |
| --- | --- | --- |
| Every "Try live demo" button | Hosted release-candidate URL. Set `DEMO_URL` in the `<script>` at the bottom of `index.html` | VDEV-024 |
| Demo video section | Fallback demo recording embed | VDEV-024 |
| Nav logo, favicon, og:image | Final logo and wordmark (currently a tree mark in a teal tile) | VBIZ-014 |
| Pricing: Free plan | Confirm that a free tier exists, and its limits | BMC |
| Pricing: Family plan | Confirm $8 CAD/mo (tested in M2 interviews), member and record limits, annual option, cancellation terms | BMC |
| Interview quotes | Two approved quotes from the caregiver interviews | Customer discovery |
| Comparison table note | Confirm the portal comparison claims | VBIZ-014 |
| FAQ: data storage | Hosting provider, encryption details, "never sell your data" policy | Dev and BCOM |
| FAQ: integrations, launch | Planned integrations, launch date or waitlist link | Team |
| Support email, Privacy, Terms | Real contact address and policy pages | Team |
