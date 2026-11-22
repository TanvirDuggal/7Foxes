# Seven Foxes

Seven Foxes is a technology consulting team helping businesses operate more reliably, automate repetitive work, improve software quality, and deliver products with greater confidence.

The team combines experience across IT support, remote monitoring and management, DevOps, infrastructure, scripting, QA, product management, and project delivery.

## Company overview

### Vision

Technology should make a business simpler, more efficient, and more dependable. Seven Foxes works as an extension of a client’s team to reduce operational overhead, improve system reliability, and support better product outcomes.

### Core services

- **IT Support & Operations** — troubleshooting, incident resolution, system administration, user support, preventive maintenance, and performance optimization.
- **RMM** — platform configuration, endpoint monitoring, alert handling, remediation, and routine maintenance automation.
- **DevOps & Infrastructure** — CI/CD pipelines, deployment automation, release support, monitoring, troubleshooting, and configuration management.
- **Scripting & Automation** — PowerShell, Python, Bash, custom IT operations scripts, workflow automation, and manual-effort reduction.
- **QA & Software Quality** — manual, functional, regression, and integration testing, plus test execution, bug verification, and release support.
- **Product Management Support** — requirements gathering, documentation, backlog prioritization, stakeholder coordination, release planning, and delivery tracking.

### Team

- **Tanvir Duggal** — 7+ years in software development, with a focus on AI.
- **Amit Pandey** — 7+ years working in cloud security and infrastructure.
- **Sanjeev Singh** — 7+ years in project management and stakeholder coordination.

The wider team includes seven experienced technology professionals with approximately 4–15 years of experience across the service areas above.

## Website

This repository contains the current static marketing website for Seven Foxes. The site presents the company vision, service capabilities, team experience, partner network placeholder, and contact call-to-action.

The site is intentionally static for now. There is no backend, database, authentication, CMS, contact form processing, or external API integration.

## Technical stack

- **HTML5** for semantic page structure and accessible content.
- **CSS3** for layout, responsive behavior, gradients, animations, cards, and theme styling.
- **Vanilla JavaScript** — currently no JavaScript runtime is required; the page is implemented without a frontend framework.
- **Local image asset** — the Seven Foxes logo is stored in `dist/assets/seven-foxes-logo.png`.
- **Google Fonts** — DM Sans and Space Grotesk are loaded from Google Fonts for the current visual system.
- **Static hosting compatible** — the output can be hosted on GitHub Pages, Cloudflare Pages, Netlify, Vercel static hosting, S3, or a standard web server.

## Project structure

```text
.
├── dist/
│   ├── index.html
│   └── assets/
│       └── seven-foxes-logo.png
└── README.md
```

The page styles are currently kept inside `dist/index.html` to keep the site portable and easy to deploy. If the site grows, the CSS can be split into `dist/styles.css` and the page can be extended with separate modules.

## Run locally

Because the site is static, it can be opened directly from the filesystem. A local HTTP server is recommended so asset paths behave the same way they will in production.

### PowerShell

From the project root:

```powershell
npx serve dist
```

Then open the local URL printed by the server.

### Alternative with Python

```powershell
python -m http.server 4173 --directory dist
```

Open `http://127.0.0.1:4173/` in a browser.

## Updating the website

1. Edit the content and styles in `dist/index.html`.
2. Replace the logo at `dist/assets/seven-foxes-logo.png` if a new brand asset is provided.
3. Keep public-facing content free of credentials, admin account details, private infrastructure information, and internal operational notes.
4. Test both desktop and mobile layouts before deployment.
5. Verify that all contact details and pricing are current before publishing.

## Content notes

- The `$10.20/hr` rate is presented as supplied and should be confirmed before publication.
- The `hello@sevenfoxes.com` email in the page is a placeholder until the company’s preferred public inbox is confirmed.
- The partner section is intentionally reserved for future partner details.
- Microsoft 365 administration details are intentionally excluded from the public site and this README.

## Deployment checklist

- Confirm the final public contact email.
- Confirm pricing, team descriptions, and service wording.
- Replace the placeholder partner content when ready.
- Test navigation anchors and the `mailto:` link.
- Confirm the logo and Google Fonts load correctly in the hosting environment.
- Deploy the contents of `dist/` as the static site root.
