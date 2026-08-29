# neeX — Portfolio & Career Roadmap Platform

A personal portfolio site with three interactive, self-contained career roadmaps — **DevSecOps**, **Full-Stack Engineering**, and **AI/ML Engineering** — each laid out as a week-by-week curriculum with topics, resources, and hands-on deliverables.

No build step, no dependencies, no backend. Plain HTML/CSS that runs anywhere a browser can open a file.

---

## 📁 Project Structure

```
.
├── index.html              # Home page — links to all three roadmaps
├── styles.css              # Home page styling
├── images/                 # Logo, social icons, domain tile images (bring your own)
│   ├── neegx.png
│   ├── twittter.png
│   ├── linkedin.png
│   ├── facebook.png
│   ├── insta.png
│   ├── github.png
│   ├── adam.png
│   ├── product.png
│   ├── swe.png
│   └── ai.png
└── routes/
    ├── devsecops.html       # DevSecOps career roadmap (24-week syllabus)
    ├── fullstack.html       # Full-Stack Engineer roadmap (9-month curriculum)
    └── aiml.html            # AI/ML Engineer roadmap (9-month curriculum)
```

> ⚠️ **Keep this folder structure intact.** All links between pages are relative (`routes/devsecops.html`, `../index.html`, `images/...`). If you move files around, update the paths or the links will break.

---

## ✨ What's Inside

- **Home page (`index.html`)** — a single-screen portfolio intro with three clickable domain tiles. Clicking a tile opens the matching roadmap in a new tab.
- **Three standalone roadmap pages** — each is a fully self-contained, dark-themed HTML document (no external JS framework) covering:
  - Phased curriculum (Beginner → Professional / Month 1 → Month 9)
  - Weekly topics, tools, resources, and deliverables in table form
  - Capstone projects per phase
  - A "← neeX home" link back to the portfolio

---

## 🚀 Getting Started Locally

No installation required.

```bash
# Clone or download the project, then just open it:
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Or use a lightweight local server (recommended, avoids any browser file:// quirks):

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## 🌍 Deploying for Free

Because this is a static site with zero build step, it can be hosted for free on any of the platforms below. Pick whichever fits your workflow.

### Option A — Netlify Drop (fastest, no Git required)

1. Make sure `index.html`, `styles.css`, `images/`, and `routes/` are together in one folder.
2. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
3. Drag the whole project folder onto the page. Netlify gives you a live URL instantly (e.g. `random-name.netlify.app`).
4. Sign up with email or GitHub to claim the site so it doesn't expire, and to redeploy later.
5. *(Optional)* Add a custom domain under **Site settings → Domain management**.

### Option B — GitHub Pages (best long-term free option)

1. Create a new **public** GitHub repository.
2. Upload `index.html`, `styles.css`, `images/`, and `routes/`, preserving the folder structure.
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. Your site publishes within a minute or two at `https://your-username.github.io/repo-name/`.
5. *(Optional)* Add a custom domain under the same Pages settings, then point your DNS at GitHub and enable **Enforce HTTPS**.

### Other free options

- **Vercel** and **Cloudflare Pages** work the same way as GitHub Pages — connect a repo, get auto-deploys on every push, free custom domain + HTTPS.
- All four options require **zero configuration** for this project — no `package.json`, no build command, just upload the files as-is.

---

## 🎨 Naming Ideas (if this grows beyond a personal portfolio)

If this ever spins out into its own standalone learning platform:

| Name | Why |
|---|---|
| **Pathforge** | Structure ("path") + effort ("forge") — short, brandable, domain-friendly |
| **Levelcraft** | Combines leveling up with hands-on craft |
| **Trackforge** | Nods to "career track" + building through labs |
| **Ramplyne** | Invented, ownable, evokes ramping up a skill line |

---

## 🛠 Tech Notes

- Pure HTML + CSS, no JavaScript framework, no build tooling.
- Each roadmap page uses its own embedded `<style>` block — they're intentionally self-contained so any one of them can be shared, copied, or hosted independently of the rest of the site.
- Social and nav links in `index.html` currently point to `#` placeholders — update `href` values once your real profiles/pages exist.
- Image assets referenced in `images/` are not included in this repo — add your own files matching the filenames above (or update the references).

---

## 📄 License & Credit

© 2026 Emeka Nwachukwu. All rights reserved unless otherwise noted.
