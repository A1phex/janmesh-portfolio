# Janmesh Thakare — Portfolio

Personal portfolio site for a systems engineer (MBSE / SysML, simulation, structural dynamics) based in Munich. Static, hand-built, bilingual (EN/DE), and deployed on GitHub Pages.

**Live:** https://a1phex.github.io/janmesh-portfolio/

---

## About

A single-page portfolio with dedicated deep-dive pages for selected engineering projects. The landing page covers background, achievements, technical skills, project summaries, recommendations, and academic record; each featured project links out to a full case-study page with derivations, code, results, and figures.

The whole site runs with no build step and no framework — plain HTML and CSS, with a small amount of vanilla JavaScript for the language toggle and smooth scrolling.

## Structure

```
janmesh-portfolio/
├── index.html                          # main landing page (EN/DE)
├── projects/
│   ├── pick-place-robot.html           # 3-DOF manipulator — IK derivation & MATLAB control
│   └── shm-vibration-simulation.html   # COMSOL + MATLAB LiveLink SHM pipeline
├── uploads/
│   ├── Bild_JanmeshThakare.jpg         # profile photo
│   └── Janmesh_Thakare_CV.pdf          # downloadable CV
└── README.md
```

## Featured projects

- **Dynamic Automatic Suppression System (DASS)** — safety-critical airbag-suppression architecture (M.Sc. thesis at BMW AG): 35 SysML requirements across four hierarchy levels, full system model, ISO 15288-compliant simulation-based verification.
- **SHM Vibration Simulation** — COMSOL Multiphysics 6.1 + MATLAB LiveLink pipeline generating synthetic vibration data for structural-health-monitoring algorithms; sssMOR model-order reduction cuts compute time 60–67%.
- **Pick-and-Place Robot** — 3-DOF manipulator with first-principles inverse kinematics and adaptive height sensing; no hard-coded positions.

## Built with

- Semantic HTML and modern CSS (OKLCH color tokens, CSS grid, `clamp()` fluid type)
- Vanilla JavaScript — bilingual content switching, smooth-scroll navigation
- Type: Space Grotesk (display) + Barlow (body), via Google Fonts
- Google Analytics 4 for visitor metrics
- Hosted on GitHub Pages

## Run locally

No dependencies or build tooling. Clone and open directly, or serve over a local web server (recommended, so relative paths resolve correctly):

```bash
git clone https://github.com/A1phex/janmesh-portfolio.git
cd janmesh-portfolio

# Python's built-in server
python -m http.server 8000
# then visit http://localhost:8000
```

## Contact

**Janmesh Thakare** — Munich, DE
[Portfolio](https://a1phex.github.io/janmesh-portfolio/) · [LinkedIn](https://www.linkedin.com/in/janmesht/) · janmesh.thakare@gmail.com
