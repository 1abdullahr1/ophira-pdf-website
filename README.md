# Ophira PDF Website ⚡

Official website and landing page for **[Ophira PDF](https://github.com/1abdullahr1/velox-desktop)** — the modern, lightning-fast, distraction-free desktop PDF reader and editor for Windows.

Built with **[Astro](https://astro.build)** and deployed automatically via **GitHub Actions** to **GitHub Pages**.

---

## 🎨 Color Palettes & Themes

The website is designed exclusively with the signature design tokens of Ophira PDF:

```css
:root {
  --brand-start: #3A34C4;  /* deep indigo (gradient start) */
  --brand-end:   #8A4FFF;  /* bright violet (gradient end) */
  --surface:     #FBFAFF;  /* near-white lavender (backgrounds, cards) */
  --shade:       #DAD6F0;  /* soft lavender-grey (borders, dividers) */
  --accent:      #FFC93C;  /* sunny yellow (buttons, highlights) */
}
```

---

## 🚀 Key Website Features

- **⚡ Blazing-Fast Astro Static Engine**: Zero client-side bloat, maximum lighthouse performance, and instant navigation.
- **🎨 Signature Color Palette**: Deep indigo, bright violet, lavender paper surface, and sunny yellow highlights matching the app icon.
- **💻 Desktop Mockup Simulator**: Interactive desktop app simulator allowing visitors to test the real in-viewer toolbar, auto-save toggle, and live status indicator.
- **💾 One-Click Downloads**: Direct download links for **Windows Setup Installer** (`Ophira.PDF.1.2.1.Setup.exe`) and **Standalone Portable** (`Ophira.PDF.1.2.1.Portable.exe`).
- **📊 In-Depth Feature Matrix**: Clear feature comparisons against sluggish legacy PDF viewers.
- **🔄 Automated GitHub Actions CI/CD**: Pushes to `main` automatically trigger GitHub Pages builds and deployment.

---

## 🛠️ Project Structure

```text
ophira-pdf-website/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow for GitHub Pages
├── public/
│   ├── favicon.svg             # Vector favicon
│   ├── favicon.ico             # Windows multi-resolution icon
│   ├── icon.png                # Master 512x512 logo
│   ├── icon-indigo.svg         # Folded-corner document icon
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── Header.astro        # Navigation + Theme Switcher
│   │   ├── Hero.astro          # Hero headline + CTA
│   │   ├── InteractiveMockup.astro # Live app preview + Auto-Save simulator
│   │   ├── Features.astro      # Core features grid
│   │   ├── ThemeShowcase.astro # Interactive color palette cards
│   │   ├── Comparison.astro    # Ophira vs legacy readers
│   │   ├── Downloads.astro     # Setup & Portable downloads
│   │   ├── FAQ.astro           # Accordion FAQ
│   │   └── Footer.astro        # Footer + theme indicators
│   ├── layouts/
│   │   └── Layout.astro        # Main layout, fonts, SEO, theme loader
│   ├── pages/
│   │   └── index.astro         # Main landing page
│   └── styles/
│       └── global.css          # Design system & CSS color tokens
├── astro.config.mjs            # Astro configuration
├── package.json
└── tsconfig.json
```

---

## 📦 Local Development (Optional)

> **Note**: As per repository guidelines, local package installation is not required. All builds and deployments are managed via GitHub Actions.

If you ever wish to develop locally:

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview build locally
npm run preview
```

---

## 📄 License

Distributed under the **MIT License**.
