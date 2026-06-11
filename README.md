# saamarth-attray.com

Personal website for Saamarth Attray — built with vanilla HTML/CSS/JS, deployed on Vercel.

## Tech

- Pure HTML, CSS, and vanilla JS (zero dependencies, zero build step)
- Animated dot-grid + light-ray canvas background
- Scroll-reveal via Intersection Observer API
- Responsive down to 375px
- Prefers-reduced-motion support

## Local development

```bash
# Serve locally — any static server works
npx serve public
# or
python3 -m http.server 8080 --directory public
```

## Deploy to Vercel

### Option A — GitHub import (recommended)
1. Push this repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import your GitHub repo
4. Vercel auto-detects `vercel.json` — click **Deploy**
5. Your site is live at `your-project.vercel.app`

### Option B — Vercel CLI
```bash
npm i -g vercel
vercel        # follow prompts
```

### Custom domain (free on Vercel)
1. Dashboard → your project → Settings → Domains
2. Add your domain → follow DNS instructions

## Customizing

All content lives in `public/index.html`. Easy places to update:

| What | Where in index.html |
|------|---------------------|
| Photo | Replace `.photo-ring` block with `<img src="photo.jpg" .../>` |
| About text | `<section id="about">` → `.about-body` paragraphs |
| Current projects | `<section id="currently">` → `.card` blocks |
| Skills chips | `<section id="skills">` → `.chips` spans |
| Contact info | `<section id="contact">` → `.contact-link` anchors |
| Tagline phrases | `phrases` array in the `<script>` at bottom |
| Status | "Open to offers" line in the info card |
