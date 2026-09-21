# Zaire Williams — Engineering Portfolio

Aerospace engineering senior at MIT. Thermal, fluid, mechanical and electrical systems for energy and space.

**Live site:** https://zwill823.github.io/zaire-williams-portfolio/

## Projects

| Project | Where | When |
|---|---|---|
| Annealing furnace for an autonomous solar-materials lab | MIT Accelerated Materials Laboratory for Sustainability | 2025 – present |
| Aeroderivative turbine repair and industrialization | GE Vernova, Greenville, SC | Summer 2026 |
| ASTEROIDS CubeSat — electronics and integration lead | MIT 16.831 | Spring 2026 |
| Autonomous soft drone | MIT SPARKLab | Fall 2024 |
| Neural-network aerodynamic shape optimization | SISSA, Trieste, Italy | Summer 2024 |

## How the site is built

The whole site is a single HTML file with no build step and no framework. Each page is a `<div class="view">`, and a small script shows one at a time based on the URL hash (`#furnace`, `#cubesat`, …). The only external dependency is Google Fonts.

The charts and diagrams are inline SVG, drawn by hand or generated from logged data, so they stay sharp at any size and need no image files.

```
index.html      the entire site: markup, styles and scripts
images/         photographs and figures
files/          downloadable documents (e.g. the ASTEROIDS flight proposal)
```

## Viewing it locally

Open `index.html` in any browser. That's it.

If a browser blocks something when opening from disk, serve the folder instead:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing

A map at the top of the `<style>` block in `index.html` points to each section: colors and fonts, navigation, pages, and photos. The résumé is embedded in the file as base64 so the link works without separate hosting. Instructions for replacing it are in the comment above the `resume-data` script tag.

## A note on the GE Vernova page

That page describes method and approach only. It contains no part identifiers, measurements or results, which remain inside GE Vernova. The surface profile viewer shown there is a layout mockup with synthetic data, not a screenshot of real traces.

## License

The source code is released under the MIT License. The written content, photographs, documents and figures are **all rights reserved**. See [LICENSE](LICENSE) for the full terms.

## Contact

zwill823@mit.edu · [LinkedIn](https://linkedin.com/in/zaireowilliams)
