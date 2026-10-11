# 3D Geometry Generation for Scientific Computing (3D4S)

Static workshop website: https://3d4sworkshop.github.io/

## Editions

- `/` and `/cfp.html`: the third edition, planned for CVPR 2027.
- `/2026/` and `/2026/cfp.html`: the second edition at CVPR 2026, with its original speakers, organizers, program, and submission information.
- [WACV 2024](https://sites.google.com/view/wacv-site-3d-geometry/home): the first edition, maintained on its original Google Site.

The root always hosts the latest edition, following the structure of the Foundation Models for Science workshop site. The CVPR 2027 theme is "3D Geometry Generation for Scientific Computing: Agentic 3D/4D Modeling for Scientific Simulation and Design." The site lists six organizers, no invited speakers yet, a proposed half-day program, and tentative dates for a non-archival CFP. Acceptance, speakers, dates, and logistics remain subject to confirmation. Research links are background reading and are not required citations.

## Keeping past editions available

Before preparing a new edition:

1. Copy the current root HTML, CSS, JavaScript, images, and downloadable files into a folder named for the outgoing year.
2. Keep the archive self-contained. Its header, footer, navigation, styles, scripts, and images use paths relative to its own folder.
3. Update the root pages for the new edition. Keep unconfirmed dates, speakers, organizers, and submission details explicitly pending.
4. Update the "Workshops by Year" menu in the root and each archived `navbar.html`. Archived section links stay within that edition; the latest-workshop link returns to the root.
5. Check both home and call-for-papers pages for each edition, including images, section anchors, and the year menu.

The 2026 archive preserves the previous site content and assets. Its navigation adds the year menu; Bootstrap uses its matching bundle so the dropdown works; template loading preserves section deep links; the missing `Styles.zip` link points to the official CVPR 2026 author guidelines and template instead.

## Local preview

Run from this directory:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000/` and `http://localhost:8000/2026/`. Use an HTTP server because the pages fetch `header.html`, `navbar.html`, and `footer.html` dynamically.

There is no build step. Publish the repository root through GitHub Pages as before.
