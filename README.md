# Telecom — Titans of Telecom: India's Telecom Battlefield

An interactive single-page dashboard that compares India's major telecom operators — **Airtel, Jio, and Vi** — side by side with charts, metric cards, and plan-comparison tables.

## Features

- **Operator comparison** — subscriber base, network speed, and market position compared with Chart.js grouped bar charts
- **5G availability insights** — doughnut charts and key metric cards for 5G rollout data
- **Plan comparison tables** — toggle between Prepaid, Postpaid, and Broadband plans and compare them interactively
- **AI Plan Finder** — a natural-language input that sends your needs and plan data to the Gemini API for a personalized plan recommendation
- **Dark-mode dashboard UI** — Tailwind CSS styling with operator brand accents, sticky nav, smooth scrolling, and responsive layout

## Tech stack

- Plain HTML / CSS / JavaScript (single `index.html`, no build step)
- [Tailwind CSS](https://cdn.tailwindcss.com) (CDN)
- [Chart.js](https://www.chartjs.org) (CDN)
- Google Fonts (Inter)
- Gemini API (optional — powers the AI Plan Finder; needs a valid API key)

## Quick start

No build step required — it's a static site:

1. Clone the repo:
   ```bash
   git clone https://github.com/girishlade111/Telecom.git
   cd Telecom
   ```
2. Open `index.html` in any browser, or serve it locally:
   ```bash
   npx serve .
   ```

## Project structure

```
.
├── index.html   # the entire dashboard (markup, styles, and JS)
└── README.md
```

## Deploy notes

Fully static — deploy anywhere that serves HTML:

- **GitHub Pages**: Settings → Pages → Deploy from branch → `main` / `/ (root)`
- Netlify / Cloudflare Pages / Vercel: drop the repo in, no build command needed

## Environment variables

- `GEMINI_API_KEY` (client-side, optional): set this in the page's script where the Gemini call is made to enable the AI Plan Finder. Without a key, everything else works.

## Author

Built by Girish Lade — https://ladestack.in
