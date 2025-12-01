# CELLDIVISION

A cutting-edge digital studio portfolio featuring WebGL fluid effects, HDR color support, and immersive visual experiences.

![Deploy Status](https://github.com/chadlittlepage/celldivision/actions/workflows/deploy.yml/badge.svg)
![Lighthouse](https://github.com/chadlittlepage/celldivision/actions/workflows/lighthouse.yml/badge.svg)

## Features

### Visual Effects
- **WebGL Fluid Cursor** - Ink-like trails that follow mouse movement
- **HDR Color Support** - Enhanced colors on Display P3 and HDR displays
- **Liquid Chrome Text** - Iridescent metallic shimmer effect
- **Neon Flicker** - Realistic neon sign with flicker animation
- **3D Extruded Text** - 16-layer shadow with hover expansion
- **Glitch Distortion** - Chromatic aberration with slice animation
- **Dripping Paint** - Animated paint drips from text

### Background Layers
- Animated gradient blobs
- 50 floating particles with glow
- CRT scanlines overlay
- Film grain/noise texture
- Mouse-following morphing blob

### Interactive Elements
- Hamburger menu with slide-out panel
- Project cards with 3D rotation
- Service cards with reveal animations
- Scroll-triggered reveals
- Parallax effects

## Tech Stack

- HTML5 / CSS3 / JavaScript (ES6+)
- WebGL via [smokey-fluid-cursor](https://www.npmjs.com/package/smokey-fluid-cursor)
- Google Fonts (Space Grotesk)

## Infrastructure

This project uses FAANG-level infrastructure:

| Service | Status | Purpose |
|---------|--------|---------|
| GitHub Actions | ✅ Active | CI/CD, Deployment |
| GitHub Pages | ✅ Active | Primary Hosting |
| Firebase Hosting | ✅ Active | Backup/CDN Hosting |
| Lighthouse CI | ✅ Active | Performance Audits |
| Dependabot | ✅ Active | Security Updates |
| Sentry | ✅ Ready | Error Tracking |

## Quick Start

```bash
# Clone the repository
git clone https://github.com/chadlittlepage/celldivision.git
cd celldivision

# Preview locally
npx http-server . -p 8080

# Open in browser
open http://localhost:8080
```

## Deployment

The site automatically deploys to GitHub Pages on every push to `main`:

**Live Sites**:
- GitHub Pages: https://chadlittlepage.github.io/celldivision
- Firebase: https://celldivision.web.app

## Performance

Optimized for 60fps on modern hardware:
- WebGL simulation resolution: 128
- HDR bloom resolution: 512
- Lazy-loaded animations
- GPU-accelerated transforms

## Browser Support

- Chrome 90+ (recommended)
- Firefox 88+
- Safari 14+
- Edge 90+

HDR features require:
- Display P3 or Rec2020 capable display
- Browser with `color-gamut` media query support

## License

Copyright 2024 Cell Division. All rights reserved.
