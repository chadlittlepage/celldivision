# CELLDIVISION - Project Context

## Project Overview
CELLDIVISION is a digital studio portfolio website featuring cutting-edge visual effects including:
- WebGL fluid cursor effects (HDR-enabled)
- Liquid chrome, neon, 3D extruded, and glitch text effects
- Animated background layers (particles, blobs, scanlines, noise)
- Scroll-triggered animations and parallax effects

## Tech Stack
- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **WebGL**: smokey-fluid-cursor library for fluid effects
- **Fonts**: Space Grotesk (Google Fonts)
- **Deployment**: GitHub Pages
- **Monitoring**: Sentry for error tracking

## Primary Color
- **Primary**: #4a556c
- **Neon Cyan**: #00ffff
- **Neon Pink**: #ff00ff

## Project Structure
```
CELLDIVISION/
├── index.html          # Main site
├── .github/
│   ├── workflows/
│   │   ├── deploy.yml      # GitHub Pages deployment
│   │   └── lighthouse.yml  # Performance audits
│   └── dependabot.yml
├── .claude/
│   └── agents/
│       ├── code-reviewer.md
│       ├── security-analyst.md
│       └── performance-auditor.md
├── CLAUDE.md           # This file
└── README.md
```

## Development Guidelines

### Performance
- Keep WebGL simResolution at 128 for balance
- Use will-change sparingly
- Prefer transform/opacity for animations
- HDR features auto-enable on capable displays

### Code Style
- Use CSS custom properties for theming
- Semantic HTML5 elements
- ES6+ JavaScript features
- Comment complex animations

### Testing
- Lighthouse audits run on every push
- Target 90+ performance score
- Test on both SDR and HDR displays

## Deployment
- **GitHub Pages**: Auto-deploys from main branch
- **Firebase Hosting**: Backup CDN deployment
- **URLs**:
  - https://chadlittlepage.github.io/celldivision (GitHub Pages)
  - https://celldivision.web.app (Firebase)

## Sentry Integration
```javascript
// Add to index.html for error tracking
<script src="https://js.sentry-cdn.com/50a16b1a705d57b1d18c6ce4d5b29f34.min.js" crossorigin="anonymous"></script>
```

Dashboard: https://sentry.io/organizations/o4510140548055040/issues/

## Commands
- Preview locally: `npx http-server . -p 8080`
- Run Lighthouse: `npx lighthouse http://localhost:8080`
