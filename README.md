<div align="center">

# `DM.` — Daksh Mahera · Portfolio

**Architect. Builder. Overthinker. Maker.**

A cinematic, single-file personal portfolio — Iron-Man "suit-up" hero, an interactive 3D globe, a hand-built custom cursor, light/dark theming, and a fully responsive layout. No frameworks, no build step. Just craft.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![No Build](https://img.shields.io/badge/build-none-brightgreen?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](#-license)

[**Live Demo →**](#) · [**Report a bug →**](#) · [**Connect →**](mailto:maheradaksh1@gmail.com)

</div>

---

## ✦ Overview

This is my personal corner of the internet — a portfolio that treats first impressions as a design problem worth solving. It opens with an interactive **"SUIT UP"** hero that assembles an Iron-Man visor over my photo, then unfolds into a scrollable story: experience, projects, a live toolkit, achievements, and the ways to reach me.

Everything lives in **one self-contained HTML file**. It's fast, portable, and hackable — open it in a browser and it just runs.

---

## ✦ Features

| | |
|---|---|
| 🦾 **Suit-up hero** | Iron-Man reveal animation — four armor panels fly in and assemble on click, with an arc-reactor glow. |
| 🌍 **Interactive globe** | A draggable, auto-rotating WebGL globe (via `cobe`) marking my base in India, with a hand-drawn canvas fallback. Re-themes instantly with the light/dark lever. |
| 🎯 **Custom cursor** | A bespoke dot-and-ring cursor with eased motion; the native pointer is fully suppressed on desktop. |
| ☀️🌙 **Light / dark theme** | A physical "lever" toggle that recolors the entire site — including the globe. |
| 🌀 **Spinning tech cloud** | A 3D icon cloud of my real stack, rendered from brand logos. |
| 📜 **Scroll choreography** | Zoom-out intros, reveal-on-scroll sections, and a running marquee of mindset + skills. |
| 📱 **Fully responsive** | Fluid `clamp()` typography, stacking layouts on mobile, and `prefers-reduced-motion` support. |
| 📄 **One-click résumé** | A download button wired to a single PDF you can swap anytime. |
| 🗂️ **Sectioned & commented** | Clearly labelled markup and an in-file editing guide so the whole thing is easy to maintain. |

---

## ✦ Tech Stack

- **Vanilla HTML5 / CSS3 / JavaScript** — zero frameworks, zero bundler.
- **[cobe](https://github.com/shuding/cobe)** — the WebGL globe.
- **[Simple Icons](https://simpleicons.org/)** — brand logos in the tech cloud.
- **Google Fonts** — `Syne` (display), `Space Grotesk` (body), `Space Mono` (labels).

---

## ✦ Getting Started

No install, no dependencies. Clone and open.

```bash
# clone
git clone https://github.com/dakshxndrm/portfolio.git
cd portfolio

# open directly...
open "Daksh Mahera Portfolio.dc.html"      # macOS
# or just double-click the file

# ...or serve locally (recommended, so fonts/assets load cleanly)
python3 -m http.server 8080
# then visit http://localhost:8080
```

> **Note:** the globe and web-fonts load from a CDN, so the first paint needs an internet connection. Everything else works offline.

---

## ✦ Project Structure

```
.
├── Daksh Mahera Portfolio.dc.html   # the entire site (markup + styles + logic)
├── image-slot.js                    # drag-and-drop image helper (achievements)
├── support.js                       # runtime
└── assets/
    ├── face.png                     # hero photo
    ├── ironman-cut.png              # suit-up overlay
    └── Daksh-Mahera-Resume.pdf      # résumé served by the Download button
```

---

## ✦ Customising It

The main file opens with a built-in **editing guide** comment that maps every section. Quick reference:

| Want to change… | Go to… |
|---|---|
| Colors / accent | `THEME TOKENS` block (top of `<style>`) — edit `--acc`, `--bg`, etc. |
| Fonts | Same token block (`--disp`, `--body`, `--mono`) + the Google Fonts `<link>`. |
| Name / headline | `<!-- ===== HERO ===== -->` |
| Experience / Projects / Achievements | The matching `<!-- ===== SECTION ===== -->`; copy any `<div data-item>…</div>` to add one. |
| Skills / toolkit | `<!-- ===== SKILLS ===== -->` for chips; `const slugs = [...]` in the script for the icon cloud. |
| Résumé | Replace `assets/Daksh-Mahera-Resume.pdf` (keep the name). |
| Links / socials | `<!-- ===== CONTACT ===== -->` |

---

## ✦ Deployment

It's static — host it anywhere:

- **GitHub Pages** — push to a repo, enable Pages on the branch.
- **Netlify / Vercel / Cloudflare Pages** — drag the folder in, or connect the repo.

Deploy the **whole folder** (the HTML file *and* the `assets/` folder together) so the photo and résumé resolve.

---

## ✦ Roadmap

- [ ] Wire up a live-demo URL badge
- [ ] Add project case-study deep-dives
- [ ] Blog / writing section
- [ ] Offline-first bundle (inline the CDN assets)

---

## ✦ Contact

**Daksh Mahera** — engineering student, relentless builder.

- ✉️ [maheradaksh1@gmail.com](mailto:maheradaksh1@gmail.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/daksh-mahera/)
- 🐙 [GitHub](https://github.com/dakshxndrm)
- 🧩 [LeetCode](https://leetcode.com/u/maheradaksh22/)

---

## ✦ License

Released under the **MIT License** — use it, learn from it, fork it. The photos, résumé, and personal content are mine; please swap those for your own.

<div align="center">

*Built with curiosity, caffeine, and a lot of `git commit --amend`.*

</div>
