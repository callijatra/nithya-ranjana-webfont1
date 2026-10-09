# Changelog

All notable changes to the **Nithya Ranjana Webfont** project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Fixed
- **Usage Section Horizontal Overflow**: Fixed a grid-track sizing bug where unbroken `@font-face` CDN URLs in `<pre>` blocks expanded the first column to ~1,142px (`min-width: auto`), pushing the second step card off-screen and causing horizontal scrolling across all viewports.
- **Grid Track Containment**: Replaced `1fr 1fr` with `repeat(2, minmax(0, 1fr))` on `.steps` and `.versions`, and added `min-width: 0; max-width: 100%` on `.step-card` and `.codebox`.
- **Code Block Scrollbars**: Added contained horizontal scrolling (`overflow-x: auto`) with styled scrollbars (`scrollbar-width: thin` and WebKit scrollbars) to `.codebox pre`.
- **Responsive Stacking**: Improved mobile breakpoint to stack `.steps` into a single column on screens &le; 900px.

### Changed
- **Specimen Slider Range**: Increased maximum font size slider from 160px to 320px in both the live specimen section (`index.html`) and the interactive studio (`demo/index.html`).
- **Header Branding**: Updated navigation header with Callijatra Foundation logo and a "Webfonts" badge linking between pages on both the landing page (`index.html`) and demo studio (`demo/index.html`).
- **Footer Brand Layout**: Refined Callijatra logo and brand presentation in the footer.

---

## [1.2.0] - 2026-10-08

### Added
- **Mobile Navigation Drawer**:
  - Animated hamburger toggle button with morphing SVG icon.
  - Collapsible mobile navigation menu with smooth height transition and staggered menu item entry animations.
  - Anchor targets mapped to page sections (`#about`, `#versions`, `#specimen`, `#usage`, demo, GitHub).
- **Callijatra Branding & Footer**:
  - Official vector logo asset added (`images/logos/callijatra_logo.svg`).
  - Comprehensive responsive footer featuring Callijatra Foundation mission, social channel links (Instagram, Facebook, YouTube, GitHub, Email) with branded hover states, and SIL OFL 1.1 licensing information.
- **Interactive Demo Links**: Direct link to the live demo studio added to `README.md` under the stylistic sets section.

---

## [1.1.0] - 2026-10-08

### Added
- **Modern Landing Homepage (`index.html`)**:
  - Script heritage showcase highlighting 8–11th century calligraphic Ranjana history.
  - Encoding cards distinguishing Devanagari Unicode (DU) and Newa Unicode (NU) editions.
  - Interactive live specimen viewer with font size slider, letter spacing adjustment, text input, and stylistic sets (`ss01`–`ss04`) toggles.
  - Curated conjunct glyph grid previewing common complex ligatures (क्ष, त्र, ज्ञ, श्र, द्ध, द्य, etc.).
  - Step-by-step implementation guide with copyable CSS declarations.
  - Theme switcher supporting light and dark modes with `localStorage` persistence and system preference detection.
  - Responsive layout with scroll-to-top floating button.

---

## [1.0.0] - 2026-10-08

### Added
- **Newa Unicode (NU) Webfonts**:
  - Bundled `NithyaRanjanaNU-Regular.woff2` and `NithyaRanjanaNU-Regular.woff` webfont files.
- **Interactive Font Studio (`demo/index.html`)**:
  - Rebuilt interactive specimen demo with live font controls (size, letter spacing, text color).
  - Presets dropdown with sample Buddhist mantras and classical texts (Maha Maya, Manjushree mantra, Prajnaparamita, etc.).
  - Live toggles for stylistic alternates (`ss01`, `ss02`, `ss03`, `ss04`).
  - Conjunct explorer and interactive specimen cards.
- **Stylesheet & Webfont Enhancements**:
  - Updated `css/nithya-ranjana.css` with `@font-face` declarations for both DU and NU webfont weights and utility classes (`.font-nithya-ranjana`, `.font-nithya-ranjana-nu`, `.font-nithya-ranjana-ss01`).

---

## [0.1.0] - 2025-12-28

### Initial Release
- Initial webfont release for Devanagari Unicode (DU) Nithya Ranjana (`NithyaRanjanaDU-Regular.woff2`, `woff`, `otf`).
- Basic demo page with font preview and size controls.
- SIL Open Font License 1.1 (`OFL.txt`).
- Project documentation and setup guide (`README.md`).
