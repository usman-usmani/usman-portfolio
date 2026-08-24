# Usman Usmani — Portfolio Website

A clean, responsive personal portfolio built with plain HTML, CSS, and JavaScript
(no frameworks, no build step) — ready to deploy to GitHub Pages or any static host.

**Live sections:** Hero · About · Skills · Experience · Projects · Certifications ·
Education · Contact

## 🗂 File structure

```
.
├── index.html          # All page content and structure
├── style.css            # Design system + responsive styles
├── script.js             # Nav toggle, scroll reveal, background animation, contact form
├── README.md
└── assets/
    ├── profile.jpg               # Profile photo
    └── Usman_Usmani_CV.pdf       # Downloadable résumé (linked from "Download Résumé")
```

## ✏️ Content source

All content (About, Skills, Experience, Projects, Certifications, Education) was
extracted directly from the attached CV (`Usman_Usmani_CV.pdf`) — nothing was
invented. Update `index.html` directly if any of the following changes:

- New projects → duplicate a `.project-card` block inside `#projects`
- New certifications → duplicate a `.cert-card` block inside `#certifications`
- New job/role → duplicate a `.timeline-item` block inside `#experience`
- Resume file → replace `assets/Usman_Usmani_CV.pdf` (keep the same filename, or
  update the `href` in the "Download Résumé" button in `index.html`)

## 🎨 Design notes

- **Palette:** deep navy background (`#0a0f1c`) with a teal accent (`#4fd1c5`) and
  a warm amber secondary accent (`#f2b84b`) — a quiet "AI systems" feel without
  leaning on generic templates.
- **Type:** Space Grotesk (display/headings), Inter (body), JetBrains Mono (labels,
  tags, metadata) — loaded from Google Fonts.
- **Signature element:** a subtle animated node-field canvas in the background,
  echoing a neural network / graph structure, tied to the AI/ML focus of the CV.
- Fully responsive down to small mobile screens; respects `prefers-reduced-motion`.

## 🚀 Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `usman-portfolio`).
2. Push these files to the repository root:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**.
4. Under **Source**, select the `main` branch and `/ (root)` folder, then **Save**.
5. Your site will be live at:
   `https://<your-username>.github.io/<repo-name>/`

No build tools or dependencies are required — it's plain static HTML/CSS/JS.

## 🔗 Editable links

| Item | Location in `index.html` |
|---|---|
| LinkedIn | `href="https://www.linkedin.com/in/usmanosmani"` (hero, about, contact) |
| Email | `mailto:osmanalee786@gmail.com` (hero, contact) |
| Résumé download | `href="assets/Usman_Usmani_CV.pdf"` (hero) |
| Certification links | each `.cert-card` `href` in `#certifications` |

## ✅ Pre-deploy checklist

- [ ] Confirm all certification links still resolve
- [ ] Replace `assets/Usman_Usmani_CV.pdf` with the latest résumé before each deploy
- [ ] Test on mobile widths (≤ 480px) and desktop
- [ ] Update graduation date in `#education` once you graduate (currently 07/2026)
- [ ] Add live-demo / GitHub links to individual `.project-card` blocks if repos are public

## 📄 License

Personal portfolio — content and photo belong to Usman Usmani.
