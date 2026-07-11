# ClimaMonitor Website

Public-facing website for the ClimaMonitor programme, hosted on GitHub Pages. Built as a static single-page site — no build step, no framework, no dependencies beyond a Google Fonts CDN import.

---

## Project Overview

ClimaMonitor is an educational and scientific platform connecting elementary and secondary schools with university researchers for real climate research. This website is the primary outreach tool for the programme, targeting school administrators, teachers, and university research partners in Czech Republic and across Europe.

The site was built during the IFSA Summer Internship 2026 by Dara Adenodi and Zachary Majeski, under the direction of Martin Tušl (ClimaMonitor founder).

---

## Repository Structure

```
/
├── index.html          # Full single-page site (HTML, CSS, JS all in one file)
├── README.md           # This file
└── images/
    ├── students-digging.jpg      # Students preparing the experimental field
    ├── students-sensor.jpg       # Students and teacher installing the weather station
    ├── teacher-instruction.jpg   # Teacher presenting the experiment outdoors
    └── sorghum-plots.jpg         # The irrigated and non-irrigated sorghum plots
```

All images must stay in the `images/` folder relative to `index.html` for the site to display them correctly.

---

## Stack

| Layer | Choice | Reason |
|---|---|---|
| HTML | HTML5, single file | No build step needed for GitHub Pages |
| CSS | Vanilla CSS with custom properties | Fast, zero dependencies, easy to edit |
| JavaScript | Vanilla JS (~30 lines) | Mobile nav toggle and workflow tooltip only |
| Fonts | Inter via Google Fonts CDN | Clean, readable at small sizes |
| Hosting | GitHub Pages | Free, static, deploys on push to main |

No React, no Vue, no Tailwind, no npm. One `index.html` file is the entire site.

---

## Sections

The page is structured as a single scrolling document with anchor-linked navigation:

- **Nav** — sticky header with logo, nav links, and Join the Program CTA
- **Hero** — headline, subheading, CTA buttons, and the ClimaMonitor model card
- **About** — programme origin, CZU partnership, and 2028 vision
- **Direct Impact on Students** — four-quadrant grid showing student outcomes
- **Research Workflow** — seven-step horizontal diagram (Research Question to Learning Phase) with hover tooltips
- **Programme Tools** — Knowledge Wiki, Live Data Portal, AI Assistant (in development)
- **Testimonials** — three quotes with a photo row below
- **2026 Pilot** — sorghum experiment timeline and pilot stats
- **ClimaMonitor for Research** — university/research partner pitch block
- **Contact** — Calendly scheduling link and direct email button
- **Footer** — programme links and contact channels

---

## Deploying to GitHub Pages

1. Push all files (including the `images/` folder) to the `main` branch of the ClimaMonitor GitHub repository.
2. Go to **Settings > Pages** in the repository.
3. Set the source to **Deploy from a branch**, select `main`, and set the folder to `/ (root)`.
4. GitHub Pages will publish the site at `https://climamonitor.github.io/<repo-name>/` within a few minutes.

If the site is being served from a subdirectory rather than the root domain, image paths may need to be prefixed. Check that `images/students-digging.jpg` resolves correctly after deployment.

---

## Making Edits

Since everything is in one file, open `index.html` in any text editor. The CSS is in the `<style>` block at the top, HTML follows, and JavaScript is at the bottom inside `<script>` tags.

**Brand colours** are defined as CSS custom properties at the top of the stylesheet and should not be changed without confirming with Martin:

```css
--green:      #158466;   /* Primary brand green */
--green-dark: #0D5C47;   /* Hover and heading green */
--green-deep: #0A3D2F;   /* Hero background, footer */
--amber:      #FFBF00;   /* Accent — use sparingly */
--blue:       #729FCF;   /* Secondary accent */
```

---

## External Links Referenced

| Label | URL |
|---|---|
| Knowledge Wiki | https://wiki.climamonitor.com/cs/home |
| Live Data Portal | https://data.climamonitor.com |
| AI Assistant (preview) | https://salmon-hill-0181f9003.7.azurestaticapps.net/ |
| LinkedIn | https://www.linkedin.com/company/climamonitor/ |
| Facebook | https://www.facebook.com/climamonitor/ |
| Calendly | https://calendly.com/climamonitor/30min?month=2026-07 |
| CZU Prague | https://www.czu.cz/en |

---

## Contact

**Martin Tušl** — Founder, ClimaMonitor s.r.o.
martin.tusl@climamonitor.com
