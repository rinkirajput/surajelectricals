# Suraj Electricals — Website Redesign

A full front-end redesign of a legacy Bootstrap/jQuery business website, rebuilt as a modern, animated, fully responsive static site — no frameworks, no build step.

**Live site:** https://surajelectricals.com

---

## Overview

The original site was a template-based Bootstrap 3 + jQuery build with dated visuals and no cohesive design system. This project redesigns it from the ground up: a custom visual identity grounded in the client's industry (electrical panel manufacturing), scroll-based animations, and a lightweight vanilla JS/CSS stack that's fast, dependency-free, and easy to host on static platforms like GitHub Pages or Cloudflare Pages.

## Key Features

- **Custom design system** — a navy + copper color palette (copper chosen to echo the copper busbars/wiring the client actually manufactures), paired with Space Grotesk, IBM Plex Sans, and IBM Plex Mono for a precise, technical feel.
- **Animated hero section** — an SVG "busbar" circuit diagram animates current flowing between nodes in the background, tying the visual language directly to the product (Power Control Centres).
- **Scroll-triggered reveals** — sections and cards fade/rise into view using `IntersectionObserver`, with staggered timing on grouped elements.
- **Animated stat readout** — key numbers count up on scroll with leading-zero formatting (`04`, `06`, `27+`) for a spec-sheet feel.
- **7-step build-process visualizer** — an animated stepper (Design → Sheet Metal → Painting → Wiring → Testing → Dispatch → Installation) with a continuously animated connecting line.
- **Infinite logo marquee** — a pure-CSS, seamless-loop scrolling strip for client logos, pausing on hover.
- **Testimonial slider** — lightweight vanilla JS carousel with autoplay and dot navigation.
- **Fully responsive navigation** — sticky nav with scroll-aware background/blur, mobile hamburger menu with slide-in panel.
- **Contact page** — includes company info cards, an embedded map, and an inquiry form.
- **Accessibility-aware motion** — every animation respects `prefers-reduced-motion`, and interactive elements have visible focus states.

## Tech Stack

- HTML5
- CSS3 (custom properties / design tokens, no framework)
- Vanilla JavaScript (`IntersectionObserver`, no libraries)
- Google Fonts (Space Grotesk, IBM Plex Sans, IBM Plex Mono)

## Project Structure

```
├── index.html                  # Homepage
├── about.html                  # About Us
├── management.html             # Management
├── products.html                # Product listing
├── power-control-centres.html   # Product detail
├── motor-control-centres.html   # Product detail
├── capacitor-panels.html        # Product detail
├── amf-panels.html              # Product detail
├── projects.html                # Projects / industries served
├── gallery.html                 # Photo gallery
├── contact.html                 # Contact + map + form
├── css/
│   └── modern.css               # Design system + all component styles
├── js/
│   └── modern.js                 # Nav, scroll reveal, count-up, slider, back-to-top
└── images/                       # Product, project, and client assets
```

## Running Locally

No build tools required — it's plain static HTML/CSS/JS.

1. Clone the repo
2. Open `index.html` directly in a browser, or serve the folder with any static server (e.g. the VS Code "Live Server" extension) for the best experience with relative paths

## Design Notes

The redesign deliberately avoids generic "dark hero + neon accent" template defaults — the copper accent color and mono-font panel-code labels (`PCC-01`, `MCC-02`, etc.) are drawn directly from the client's actual product line and industry terminology, so the visual language stays grounded in what the company does rather than being decorative for its own sake.

---

## Credits

Designed & developed by **Rinki Rajput**
[GitHub](https://github.com/rinkirajput/surajelectricals)