# Janmesh Thakare — Portfolio

Personal portfolio site. German-first, bilingual (DE/EN), static, hand-built, deployed on GitHub Pages.

**Live:** https://a1phex.github.io/janmesh-portfolio/

---

## About

A single page carrying two tracks of the same capability — Systems Engineering and product/project work — as one method described twice, rather than two competing halves. Anchor navigation, no routing, no build step, no framework. Two deep-dive pages for selected university engineering projects link out from the capabilities section.

## Structure

```
janmesh-portfolio/
├── index.html                          # the site: markup, inline CSS, DE/EN dictionary
├── projects/
│   ├── pick-place-robot.html           # 3-DOF manipulator — IK derivation & MATLAB control
│   └── shm-vibration-simulation.html   # COMSOL + MATLAB LiveLink SHM pipeline
├── uploads/
│   ├── Bild_JanmeshThakare.jpg         # profile photo
│   └── og-image.png                    # Open Graph link preview card
└── README.md
```

Sections, in order: Hero · Zwei Perspektiven eine Methode · Arbeiten · Kompetenzen · Wie ich mit KI arbeite · Über mich · Referenzen · Kontakt.

## Design system

All values live in one `:root` token block and are reused throughout; new sections introduce no new colours, font families or radii.

- **Colour** — OKLCH, one neutral ramp on hue 242 plus a single accent (`--am`, hue 255). No shadows anywhere; elevation is a white surface on a tinted background with a 1px border.
- **Type** — Space Grotesk (display, labels, UI) + Barlow (body prose). Uppercase accent labels at .64–.68rem with .2em tracking.
- **Radius** — 3px, used exactly once. Everything else is square.
- **Rhythm** — universal `clamp(20px, 7vw, 108px)` gutter; eyebrow → 14px → H2 → 48px → content.
- **Breakpoints** — 600px (nav), 720px (two-column grids), 840px (hero).

## Content rules

- Every factual claim traces to a verified source. Nothing is filled in with plausible-sounding copy.
- The master's thesis carries a confidentiality restriction (Sperrvermerk) until 20 May 2035: methodology and headline counts only, no model screenshots, no parameter values, no internal naming. One reference quote is published as an excerpt for the same reason.
- The scheduling tool never names the employer or the airport, and carries no real names, rosters or shift data.
- German is authoritative; English is a translation of the German.

## Accessibility & performance

Lighthouse (mobile emulation, local): **performance 94, accessibility 100, best practices 100, SEO 100.** Total page weight 151 KiB.

Semantic heading hierarchy with a single `h1`, `main` landmark, skip link, visible focus rings, and `prefers-reduced-motion` respected. No analytics, no cookies, no third-party tracking — only Google Fonts is requested cross-origin.

## Run locally

No dependencies or build tooling. Serve over a local web server so relative paths resolve:

```bash
git clone https://github.com/A1phex/janmesh-portfolio.git
cd janmesh-portfolio
python -m http.server 8000
# then visit http://localhost:8000
```

## Contact

**Janmesh Thakare** — Munich, DE
[Portfolio](https://a1phex.github.io/janmesh-portfolio/) · [LinkedIn](https://www.linkedin.com/in/janmesht/) · janmesh.thakare@gmail.com
