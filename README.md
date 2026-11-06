# Vitalitree Landing Page (VDEV-023)

A single static `index.html` file with no build step and no dependencies. The only external request loads Atkinson Hyperlegible from Google Fonts.

The app itself lives in [Vitalitree-App](https://github.com/SENG455-Vitalitree/Vitalitree-App). This history was moved here from that repo's `landing/` folder ([PR #46](https://github.com/SENG455-Vitalitree/Vitalitree-App/pull/46)).

The design tokens (colours, type, radius, spacing) come from the POC style guide (`Vitalitree-POC/Style Guide.pdf`). The phone mockups are rebuilt in HTML to match the app's current screens and demo personas (Patient Patricia and Caring Carly).

Pricing, hosting and privacy claims come from the team's Startup Studio doc and the M3 Business Model Canvas. Update the page if those change.

The logo lives in `assets/`: `logo-160.png` (nav and footer), `logo-512.png` (social preview) and `favicon.png`.

## Preview locally

```bash
open index.html
```

## Deploy

Any static host works. The site is the repo root, with no build step.

- **GitHub Pages**: in repo Settings → Pages, choose "Deploy from a branch", select `main` and `/ (root)`. The site is served at `https://seng455-vitalitree.github.io/Vitalitree-Landing/`.
- **Netlify / Vercel**: create a new site from this repo and leave the build command and output directory empty.

## Live Demo (VDEV-024)

The live mobile demo is deployed at `https://vitalitree-app.expo.app/` and accessible via the QR code (`WEB_QR.svg`) in `<section id="demo">`.

Once the site has a domain, change `og:image` in the `<head>` to an absolute URL so link previews show the logo.

## Left off on purpose

These were removed because the team doesn't have them yet. Add them back when they exist:

- A support email or contact form (the FAQ section had a contact card)
- Privacy policy and Terms of use pages (footer links)
- Free plan limits in numbers (the page uses the BMC wording: one profile, a small care circle, limited storage)
