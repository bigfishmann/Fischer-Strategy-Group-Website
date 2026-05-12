[README.md](https://github.com/user-attachments/files/27652197/README.md)
# Fischer Strategy Group — Website

**Live site:** [fsg-us.com](https://fsg-us.com)  
**Hosted on:** Cloudflare Pages  
**Built with:** HTML, CSS, JavaScript (single file, no dependencies)

---

## Overview

This is the official website for Fischer Strategy Group, a revenue strategy consultancy founded by Brian Fischer. The site is a single self-contained HTML file (`index.html`) with all styles, scripts, and assets (including the headshot image) embedded inline.

---

## Site Structure

The site is a single-page application with five sections navigated via the top menu:

| Page | Description |
|------|-------------|
| **Home** | Hero, core services overview, Vision/Execute/Scale framework |
| **Services** | Overview of all four service areas with individual detail pages |
| **Testimonials** | Client testimonials (currently placeholder — coming soon) |
| **About** | Founder bio and career history (currently placeholder — coming soon) |
| **Let's Talk** | Contact form wired to Formspree (endpoint: `meennbnv`) |

---

## Services

1. **Go-To-Market Strategy** — ICP definition, pipeline architecture, sales org design, founder-led sales transformation
2. **AI-Enabled Revenue Operations & Sales Transformation** — AI workflow integration, RevOps modernization, GTM process optimization
3. **Executive Recruiting & Revenue Leadership Search** — VP Sales, CRO, enterprise AE recruiting
4. **Founder & Revenue Leadership Advisory** — Operator advisory for founders and revenue leaders

---

## Contact Form

The contact form uses **Formspree** to deliver submissions to brian@fsg-us.com.

- **Formspree endpoint:** `https://formspree.io/f/meennbnv`
- **Library:** `@formspree/ajax@1` loaded via CDN (no install required)
- **Fields:** Name, Email, Phone, Company, Company Website, Message

To update the Formspree endpoint, search for `meennbnv` in `index.html` and replace both instances with your new form ID.

---

## Making Updates

All content lives in `index.html`. Common updates:

**Changing text content**
Open `index.html`, use Ctrl+F / Cmd+F to find the text you want to change, edit it, and save.

**Updating the headshot**
The headshot is embedded as a base64 string. To swap it out:
1. Convert your new image to base64 (use a tool like [base64.guru](https://base64.guru))
2. Search for `data:image/jpeg;base64,` in `index.html`
3. Replace the base64 string that follows with your new one

**Adding testimonials**
In `index.html`, find the testimonials page section (search for `page-testimonials`) and add testimonial cards using the existing HTML structure as a template.

**Updating contact info**
Search for `brian@fsg-us.com` to find and update email references. Search for `brian-m-fischer` to update the LinkedIn URL.

---

## Deployment

The site deploys automatically via **Cloudflare Pages** on every commit to the `main` branch.

| Setting | Value |
|---------|-------|
| Build command | *(none)* |
| Build output directory | *(none)* |
| Root directory | `/` |

To deploy a change:
1. Edit `index.html` in this repository
2. Commit to `main`
3. Cloudflare Pages will redeploy automatically (typically within 60 seconds)

---

## Tech Stack

| Component | Technology |
|-----------|------------|
| Markup & layout | HTML5 / CSS3 |
| Interactivity | Vanilla JavaScript |
| Fonts | Google Fonts (Cormorant Garamond, Barlow, Barlow Condensed) |
| Form handling | Formspree (`@formspree/ajax`) |
| Hosting | Cloudflare Pages |
| Version control | GitHub |

---

## Brand

| Element | Value |
|---------|-------|
| Primary color | `#0d1f3c` (Navy) |
| Accent color | `#c9a84c` (Gold) |
| Silver | `#c8d4e0` |
| Tagline | Vision \| Execute \| Scale |

---

## Contact

**Brian Fischer**  
Founder, Fischer Strategy Group  
brian@fsg-us.com  
[linkedin.com/in/brian-m-fischer](https://linkedin.com/in/brian-m-fischer)  
San Francisco, CA
