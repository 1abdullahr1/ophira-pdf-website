# Ophira PDF Website ⚡

Official website and landing page for **[Ophira PDF](https://github.com/1abdullahr1/velox-desktop)** — the modern, lightning-fast, distraction-free desktop PDF reader and editor for Windows.

Built with **[Astro](https://astro.build)** and deployed automatically via **GitHub Actions** to **GitHub Pages**.

---

## 🎨 Color Palettes & Themes

The website features an interactive theme switcher powered by the exact design tokens of Ophira PDF:

```css
:root,
[data-theme="indigo"] {
  --brand-start: #3A34C4;
  --brand-end:   #8A4FFF;
  --surface:     #FBFAFF;
  --shade:       #DAD6F0;
  --accent:      #FFC93C;
}

[data-theme="emerald"] {
  --brand-start: #0D3B36;
  --brand-end:   #0D3B36;
  --surface:     #F5F2E9;
  --shade:       #DDD8CA;
  --accent:      #FF7B54;
}

[data-theme="navy"] {
  --brand-start: #1B2532;
  --brand-end:   #1B2532;
  --surface:     #F6F4EF;
  --shade:       #E0DED8;
  --accent:      #FCBB1B;
}

[data-theme="light"] {
  --brand-start: #CFE0F3;
  --brand-end:   #CFE0F3;
  --surface:     #FFFFFF;
  --shade:       #D3DCE8;
  --accent:      #FCBB1B;
}
```

---

## 🚀 Key Website Features

- **⚡ Blazing-Fast Astro Static Engine**: Zero client-side bloat, maximum lighthouse performance, and instant navigation.
- **🎨 Live Interactive Theme Switcher**: Instant switching between Indigo, Emerald, Navy, and Light with persistent `localStorage` memory and zero flash of unstyled content.
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
