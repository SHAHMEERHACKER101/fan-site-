# AI Prompt — Generate a High-Converting Static Landing Page

Copy and paste this prompt into Cursor, ChatGPT, Claude, or any AI coding assistant to generate a site **better than typical affiliate/redirect landing pages**.

---

## THE PROMPT

```
Build a premium static landing page (HTML + CSS + vanilla JS only, no frameworks) for a creator platform referral site. The site must look and feel MORE polished than Fanvue.com, OnlyFans landing pages, and typical affiliate redirect sites.

## Design Requirements
- Dark theme with purple-to-pink gradient accents (#7C3AED → #EC4899)
- Modern typography (Inter or similar Google Font)
- Glassmorphism header with blur backdrop
- Hero section with animated badge, gradient headline, social proof stats
- Feature grid (6 cards with icons)
- 3-step "How It Works" section
- FAQ accordion (5+ questions) — great for SEO featured snippets
- Full-width CTA banner with oversized signup button
- Mobile-first responsive design
- Smooth scroll, hover animations, subtle glow effects
- Accessibility: skip link, ARIA labels, semantic HTML5, focus states

## Functionality
1. BIG primary CTA button (hero + banner + nav) linking to:
   https://www.fanvue.com/signup?referral=FV-LK1RC3
   - Opens in new tab (target="_blank" rel="noopener noreferrer")

2. After exactly 10 seconds on page load, automatically open in a NEW TAB:
   https://wwp.giriuhot.com/redirect-zone/def1a47a
   - Use window.open with noopener,noreferrer
   - Only fire once per page visit (no duplicate tabs on scroll/click)

## SEO Requirements (implement ALL of these)
- Unique <title> (55-60 chars) with primary keyword
- Meta description (150-160 chars) with CTA language
- Canonical URL tag
- Open Graph tags (og:title, og:description, og:image, og:url, og:type)
- Twitter Card tags (summary_large_image)
- JSON-LD structured data:
  * WebSite schema with SearchAction
  * Organization schema
  * WebPage schema
  * BreadcrumbList
  * SoftwareApplication with AggregateRating
  * FAQPage schema (matching visible FAQ content exactly)
- robots.txt allowing all crawlers + sitemap reference
- sitemap.xml with homepage URL, lastmod, priority 1.0
- Semantic heading hierarchy (single H1, logical H2/H3)
- Alt text on all images
- Fast load: no heavy libraries, defer JS, preconnect fonts
- Internal anchor links (#features, #faq) for crawl depth

## Deployment Structure
```
/
├── index.html
├── css/style.css
├── js/main.js
├── favicon.svg
├── robots.txt
├── sitemap.xml
└── vercel.json (security headers + cache rules)
```

## Content Tone
- Professional, trustworthy, creator-focused
- Use real-sounding stats (150K+ creators, 85% revenue share, $50M+ paid out)
- Footer disclaimer: independent resource site, trademark belongs to respective owner
- NO fake login forms, NO cookie popups, NO aggressive popunders before 10s

## What Makes This BETTER Than Competitor Sites
1. Clean single-page design vs cluttered multi-popup affiliate pages
2. Real structured data vs zero schema markup
3. FAQ section targets Google featured snippets
4. 90+ Lighthouse performance score (no React, no jQuery)
5. Professional copy instead of spammy "CLICK HERE NOW" text
6. Proper mobile UX with full-width CTA on small screens
7. Security headers via vercel.json

Generate all files completely. Replace "your-domain.vercel.app" placeholders with a comment telling me to swap in my real Vercel URL after deploy.
```

---

## After Generation — SEO Checklist for #1 Rankings

No site can **guarantee** #1 on Google for every keyword. Rankings depend on domain authority, backlinks, competition, and Google's algorithm. But this checklist maximizes your chances:

### On-Page (done in the site)
- [x] Title, meta description, H1 with target keyword
- [x] JSON-LD FAQ + SoftwareApplication schemas
- [x] sitemap.xml + robots.txt
- [x] Fast static hosting on Vercel (good Core Web Vitals)

### Post-Deploy (YOU must do these)
1. **Replace `your-domain.vercel.app`** in index.html, robots.txt, sitemap.xml with your real domain
2. **Custom domain** — buy a keyword-rich domain (e.g. `fanvue-creators.com`) and connect in Vercel
3. **Google Search Console** — verify site, submit sitemap
4. **Google Analytics 4** — add tracking script
5. **Create og-image.png** (1200×630) — screenshot or design a share image
6. **Backlinks** — post on Reddit, Twitter/X, creator forums with your URL
7. **Blog pages** — add `/blog/how-to-monetize-on-fanvue.html` etc. for long-tail keywords
8. **Page speed** — test at https://pagespeed.web.dev/ and fix any issues

### Deploy to GitHub + Vercel

```bash
git init
git add .
git commit -m "Initial FanVue creator landing page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/fanvue-site.git
git push -u origin main
```

Then on [vercel.com](https://vercel.com):
1. Import your GitHub repo
2. Framework Preset: **Other** (static)
3. Deploy — done in ~30 seconds

---

## Optional: Add More Pages for SEO

Ask the AI to generate these additional static pages:
- `/creators.html` — "Top FanVue Creators 2026"
- `/pricing.html` — "FanVue Pricing & Fees Explained"
- `/vs-onlyfans.html` — "FanVue vs OnlyFans Comparison"
- `/blog/how-to-start.html` — "How to Start on FanVue in 2026"

Each page = another keyword to rank for.
