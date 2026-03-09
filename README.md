# Elena — Data Scientist Portfolio

A modern, responsive portfolio landing page built for a data scientist. Designed to showcase technical projects, skills, and professional experience with a clean, visually striking aesthetic that stands out to recruiters and hiring managers.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## Live Preview

Open `index.html` in any modern browser — no build step required.

## Features

- **Fully responsive** — mobile-first design that works across all breakpoints
- **Smooth scroll animations** — Intersection Observer-based reveal effects with staggered delays
- **Micro-interactions** — custom cursor, hover transforms, animated scroll indicator, loading screen
- **SEO optimized** — semantic HTML5, Open Graph tags, Twitter Card meta, descriptive ARIA labels
- **Accessible** — keyboard navigation, focus-visible outlines, `prefers-reduced-motion` support, proper heading hierarchy
- **Performance** — zero dependencies (fonts only), no framework overhead, passive event listeners
- **Themeable** — all colors, fonts, spacing, and radii controlled via CSS custom properties

## Sections

| Section | Description |
|---------|-------------|
| **Hero** | Full-viewport intro with animated background orbs, gradient text, and CTA buttons |
| **About** | Bio, profile photo placeholder, and key stats (years, projects, publications) |
| **Skills** | 6 skill cards covering ML, NLP, deep learning, data engineering, MLOps, and statistics |
| **Tech Ticker** | Auto-scrolling marquee of technologies |
| **Projects** | 4 featured projects with CSS mockup screenshots, tech tags, and links |
| **Experience** | Timeline of 4 roles with descriptions and skill tags |
| **Contact** | Split layout with social links + contact form |https://github.com/GianCarlos25/portfolio-landing-templates.git

## Tech Stack

- **HTML5** — semantic elements (`<section>`, `<article>`, `<nav>`, `<footer>`)
- **CSS3** — custom properties, grid, flexbox, `clamp()`, `backdrop-filter`, gradient text, keyframe animations
- **Vanilla JavaScript** — Intersection Observer API, scroll listeners, mobile navigation toggle, form handling
- **Google Fonts** — Inter (sans-serif) + JetBrains Mono (monospace)

## Color Palette

| Variable | Hex | Usage |
|----------|-----|-------|
| `--color-primary` | `#c47a5a` | Warm copper — headings, accents, CTAs |
| `--color-primary-light` | `#d4956e` | Links, hover states |
| `--color-bg` | `#0e0e11` | Page background |
| `--color-bg-card` | `#1c1c21` | Card surfaces |
| `--color-accent-teal` | `#5ab8a0` | Secondary accent |
| `--color-accent-purple` | `#9d7cd8` | Tertiary accent |
| `--color-accent-rose` | `#d97777` | Warning/highlight accent |

## Customization

### Change the color theme

Edit the CSS custom properties in `:root` at the top of the `<style>` block:

```css
:root {
  --color-primary: #c47a5a;      /* change to your brand color */
  --color-primary-light: #d4956e;
  --color-primary-dark: #a5603f;
  /* ... */
}
```

### Replace content

All content is in plain HTML — search and replace names, descriptions, and project details directly in `index.html`. Key areas:

1. **Hero section** — name, tagline, CTA text
2. **About section** — bio paragraphs, stats
3. **Skills cards** — titles, descriptions, technology tags
4. **Project cards** — titles, descriptions, tech stacks, links
5. **Experience timeline** — roles, companies, dates, bullet points
6. **Contact section** — email, social links
7. **Meta tags** — `<title>`, `og:` tags, `twitter:` tags

### Add a real profile photo

Replace the `.about__image-placeholder` div with an `<img>` tag:

```html
<div class="about__image">
  <img src="photo.jpg" alt="Elena Vargas" loading="lazy">
</div>
```

### Add real project screenshots

Replace the `.project-mockup` divs inside `.project-card__image-inner` with actual images:

```html
<div class="project-card__image-inner">
  <img src="project-screenshot.png" alt="Project name screenshot" loading="lazy">
</div>
```

## Performance Notes

- **No external JS dependencies** — everything runs on vanilla JavaScript
- **Fonts loaded with `display=swap`** — prevents invisible text during load
- **Passive event listeners** — scroll handlers don't block the main thread
- **IntersectionObserver** — animations only trigger when elements enter the viewport
- **`prefers-reduced-motion`** — automatically disables animations for users who prefer it

## Browser Support

Tested on Chrome, Firefox, Safari, and Edge (latest versions). Graceful degradation for older browsers via standard CSS fallbacks.

## License

MIT — free to use, modify, and distribute.
