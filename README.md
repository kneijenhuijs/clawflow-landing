# ClawFlow Landing Page

Landing page for [ClawFlow](https://kneijenhuijs.github.io/clawflow-landing/) — the productivity system for OpenClaw.

## Live Site

**URL:** https://kneijenhuijs.github.io/clawflow-landing/

## Tech Stack

- Single HTML file (fast, no build step)
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- [Inter](https://fonts.google.com/specimen/Inter) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) fonts
- Deployed via GitHub Pages (main branch)

## Local Development

```bash
# Just open the file
open index.html

# Or serve locally
python3 -m http.server 8000
# → http://localhost:8000
```

## Deployment

The site deploys automatically via GitHub Pages from the `main` branch.

To deploy manually:
```bash
git add .
git commit -m "Update landing page"
git push origin main
```

GitHub Pages will pick up the changes within 1-2 minutes.

## Structure

```
├── index.html          # Landing page (single file)
├── README.md           # This file
└── CNAME               # Custom domain (if configured)
```

## TODO

- [ ] Connect email form to ConvertKit/Mailchimp/Buttondown
- [ ] Add Gumroad buy button when paid template launches (April 10)
- [ ] Add OG image (`og-image.png`)
- [ ] Add testimonials section after free skill launch
- [ ] Custom domain setup (clawflow.com or similar)

## Email Form

The email capture form currently stores submissions in `localStorage` as a placeholder. Before launch, connect it to your email service:

### ConvertKit
Replace the form `onsubmit` handler with:
```html
<form action="https://app.convertkit.com/forms/YOUR_FORM_ID/subscriptions" method="post">
```

### Buttondown
```html
<form action="https://buttondown.com/api/emails/embed-subscribe/YOUR_USERNAME" method="post">
```

## SEO

- Schema.org `SoftwareApplication` markup included
- Open Graph + Twitter Card meta tags
- Target keywords: "OpenClaw productivity", "AI productivity system", "knowledge worker automation"

## Related

- [ClawFlow Launch Playbook](../ClawFlow-Launch-Playbook.md)
- [Messaging Strategy](../Marketing/clawflow-messaging-strategy.md)
- [ClawFlow Free Skill](../Free-Skill/)

---

**Built by [Dr. Data Science](https://drdata.science)**
