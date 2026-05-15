[PORTFOLIO_README.md](https://github.com/user-attachments/files/27814102/PORTFOLIO_README.md)
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=160&section=header&text=Sumit%20Upadhyay%20–%20Portfolio&fontSize=36&fontColor=fff&animation=fadeIn&fontAlignY=38" />

# 🌐 Personal Portfolio Website

**A sleek, dark-themed portfolio with live EN ↔ DE language switching**

[![Live Demo](https://img.shields.io/badge/🔗_Live_Demo-000000?style=for-the-badge)](https://sumit-upadhya-y.github.io/My_website/)
[![Made With HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](/)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

</div>

---

## ✨ Features

- 🎨 **Dark data-tech design** — Deep navy background with electric cyan & violet gradients
- 🌍 **Live EN ↔ DE translation** — One-click German/English toggle, zero external APIs, all 200+ strings translated in-browser
- ⌨️ **Animated typing hero** — Cycles through job titles in both languages
- 📊 **Animated skill bars** — Progress bars fire on scroll into view
- 🏅 **15-cert grid** — All LinkedIn certifications displayed with colour-coded icons
- 📱 **Fully responsive** — Works on mobile, tablet and desktop
- ⚡ **Zero dependencies** — No npm, no frameworks, no build step — pure HTML/CSS/JS
- 🔎 **Scroll-reveal animations** — IntersectionObserver-powered fade-in on every section
- 🗂️ **6 sections**: Hero · About · Resume · Projects · Certifications · Contact

---

## 📸 Sections Overview

| Section | What's Inside |
|---------|--------------|
| **Hero** | Name, animated typing role, LinkedIn & GitHub CTAs, scroll indicator |
| **About** | Personal card with animated skill bars, tech tags, bio paragraphs |
| **Resume** | Timeline of work experience + education + certification preview |
| **Stats** | 12+ projects · 1.5+ years · 15+ certs · 20+ workshops |
| **Projects** | Job Market SQL · IPL Auction SQL · Fitbit Excel — all linked to GitHub |
| **Certifications** | Full 15-cert grid with issuer, date, colour-coded category icons |
| **Contact** | Location · Email · CV download · LinkedIn |

---

## 🚀 Getting Started

No installation or build required.

### Option 1 — Open locally
```bash
# Clone the repo
git clone https://github.com/Sumit-Upadhya-y/My_website.git

# Open in browser
open index.html
# or just double-click index.html
```

### Option 2 — Deploy to GitHub Pages (recommended)
```bash
# 1. Go to your repo Settings → Pages
# 2. Source: Deploy from a branch
# 3. Branch: main  /  Folder: / (root)
# 4. Save — live in ~60 seconds at:
#    https://Sumit-Upadhya-y.github.io/My_website/
```

---

## 🗂️ File Structure

```
My_website/
│
├── index.html          # ← Single-file app: all HTML + CSS + JS
└── README.md           # ← This file
```

> All styles and scripts are embedded in `index.html` for maximum portability — no external files needed.

---

## 🌍 Language Toggle

The EN ↔ DE toggle is powered by a hardcoded `i18n` object in plain JavaScript:

```js
const i18n = {
  en: { hero_badge: "Available for Werkstudent roles · Trier, Germany", ... },
  de: { hero_badge: "Offen für Werkstudentenstellen · Trier, Deutschland", ... }
};

function toggleLang() {
  currentLang = currentLang === 'en' ? 'de' : 'en';
  document.querySelectorAll('[data-i18n]').forEach(el => {
    el.textContent = i18n[currentLang][el.dataset.i18n];
  });
}
```

Every translatable element carries a `data-i18n="key"` attribute. No external API, no latency.

---

## 🎨 Design Tokens

| Token | Value | Used For |
|-------|-------|----------|
| `--bg` | `#080c14` | Page background |
| `--accent` | `#00d4ff` | Electric cyan highlights |
| `--accent2` | `#7c5cfc` | Violet gradient |
| `--gold` | `#f5c542` | Typing text, grade badges |
| `--font-h` | Syne | All headings |
| `--font-b` | DM Sans | Body text |
| `--font-m` | DM Mono | Labels, chips, code |

---

## 🛠️ Built With

- **HTML5** — Semantic structure
- **CSS3** — Custom properties, Grid, Flexbox, animations, `@keyframes`
- **Vanilla JavaScript** — i18n engine, typing animation, IntersectionObserver scroll-reveal
- **Google Fonts** — Syne · DM Sans · DM Mono

---

## 📋 Customisation Guide

To adapt this portfolio for yourself, edit these sections in `index.html`:

| What to change | Where |
|----------------|-------|
| Name, email, links | `<!-- HEADER -->` section + `i18n` object |
| Skills & percentages | `.skill-fill` elements in About section |
| Work experience | `<!-- RESUME -->` timeline items |
| Projects | `<!-- PROJECTS -->` cards (title, desc, GitHub URL) |
| Certifications | `<!-- CERTIFICATIONS -->` cert-card items |
| German translations | `i18n.de` object in `<script>` block |

---

## 📄 License

This project is open source under the [MIT License](LICENSE).  
Feel free to fork, adapt, and use it for your own portfolio — a ⭐ star is appreciated!

---

<div align="center">

**Made with 💙 by [Sumit Upadhyay](https://www.linkedin.com/in/sumitupadhyay815)**

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=80&section=footer" />

</div>
