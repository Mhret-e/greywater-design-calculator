# Greywater Treatment System — Interactive Design Calculator (UAE)

An interactive, browser-based design calculator for decentralized, solar-powered greywater treatment systems in residential UAE households. Built as a single self-contained web app — no installation, no backend, no build step.

🔗 **Live demo:**[ _add your GitHub Pages link here once enabled_](https://mhret-e.github.io/greywater-design-calculator/)

---

## What it does

The calculator walks through six linked modules, each feeding into the next:

| # | Module | What it calculates |
|---|--------|---------------------|
| 1 | **Flow & Sizing** | Household greywater generation, stream split (shower/ablution/laundry/washbasin), design influent flow, toilet-flushing demand and surplus |
| 2 | **Energy Demand** | Daily electrical load of controller, sensors, pumps, valves, and dosing system, with a configurable design margin |
| 3 | **Solar PV & Battery Sizing** | Recommended PV array size and battery capacity based on peak sun hours (winter/summer/annual) and autonomy days |
| 4 | **Cost & Payback** | Capital cost estimate, annual water-bill savings, simple and net payback period, 15-year cumulative savings chart |
| 5 | **Water Quality & Control** | Live compliance check of pH, BOD₅, TSS, turbidity, residual chlorine, dissolved oxygen, and microbiological parameters against P1 (unrestricted) / P2 (restricted) reuse standards, plus chlorine-dosing simulation |
| 6 | **Process Flow** | Visual flow diagram showing whether treated water proceeds to storage or is recirculated for further treatment |

All inputs are adjustable sliders/fields — every value updates live across all six modules. Results can be exported as CSV or printed as a summary sheet.

---

## Tech stack

- Vanilla HTML, CSS, and JavaScript — no framework, no build step
- [Chart.js](https://www.chartjs.org/) (loaded via CDN) for the visualizations
- Fully static — works offline once loaded, deployable anywhere that serves static files

---

## Running it

**Locally:** just open `docs/index.html` in any modern browser. No server, no dependencies to install.

**Hosted:** this repo is set up for GitHub Pages — see [Deploying](#deploying-with-github-pages) below.

---

## Repository structure

```
greywater-design-calculator/
├── README.md
├── .gitignore
└── docs/
    └── index.html      ← the calculator (GitHub Pages serves from here)
```

---

## Deploying with GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select **Deploy from a branch**
4. Branch: `main`, folder: `/docs` → **Save**
5. GitHub will publish it at `https://<your-username>.github.io/greywater-design-calculator/` within a minute or two

---

## Background

This tool was built alongside ongoing research into solar-powered, sensor-monitored greywater treatment systems for non-potable residential reuse in the UAE. Citation and link to the associated paper will be added here once available.

---

## Disclaimer

This tool projects expected performance and costs based on literature-reported values and stated engineering assumptions. It is a design aid, not a substitute for laboratory or field testing.
