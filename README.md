# Aura: Premium Headphones Landing Page

> Hear everything. Block out the rest.

![Status](https://img.shields.io/badge/status-live-brightgreen)
![HTML](https://img.shields.io/badge/html-5-E34F26)
![CSS](https://img.shields.io/badge/css-3-1572B6)
![JavaScript](https://img.shields.io/badge/javascript-vanilla-F7DF1E)

**Live site: [aura-headphones-may21-2026.vercel.app](https://aura-headphones-may21-2026.vercel.app)**

---

## What It Is

Aura is a concept landing page for a premium headphones brand. Fifth project overall, first built as pure HTML/CSS/JS with no framework. The brief was to build something scroll-driven and interactive, closer to an Apple-style product microsite than a standard marketing page.

Built with Claude Design, deployed on Vercel.

---

## How It Works

The page is a single HTML file. No build step, no dependencies, no npm. Everything runs in the browser.

**Snap scroll** via CSS scroll-snap-type: y mandatory. Each section locks into place as you scroll, like flipping through a book. Twelve sections total.

**Reveal animations** trigger when each section snaps into view. Elements start at opacity 0 and translateY 28px, then transition in with staggered delays.

**3D headphone models** via two Spline embeds. The hero uses an interactive Bose colorizer scene where you can drag and change colors in real time. The immersive sound section uses a full product showcase scene.

**Custom cursor** is a glowing blue dot with a lagged ring that follows behind it. Scales up on hover.

**ANC visualizer** in the noise cancellation section generates 40 animated bars that suppress themselves when the section snaps into view, showing the noise cancellation concept visually.

**Spatial audio visualizer** animates 6 dots orbiting a center point at different speeds and radii, representing the 3D audio positioning system.

**Keyboard navigation** via arrow keys, Page Up/Down, Home, End.

**Navigation dots** on the right side show which section you're on. Each dot has a label tooltip on hover.

---

## Sections

1. Hero: interactive 3D headphone colorizer, headline, CTAs
2. Features: 40hr battery, ANC Pro, Hi-Res Audio
3. Immersive Sound: spatial audio section with 3D product showcase
4. ANC: animated noise cancellation visualizer
5. Spatial Audio: orbiting dots animation
6. Battery: animated battery fill
7. Materials: aluminium and leather texture panels
8. Specs: driver, frequency, impedance, weight, bluetooth
9. Testimonial 01
10. Testimonial 02
11. Testimonial 03
12. Final CTA: buy now

---

## Tech

| Layer | Detail |
|-------|--------|
| Markup | HTML5 |
| Styling | Vanilla CSS with custom properties |
| Animation | CSS transitions + vanilla JS |
| 3D scenes | Spline embeds via iframe |
| Fonts | Syne, DM Sans, JetBrains Mono (Google Fonts) |
| Deployment | Vercel |

---

## What I Learned

Pure HTML/CSS/JS is underrated. No React, no build step, no node_modules. The snap scroll behavior, custom cursor, intersection observers, and all the animations are just browser APIs. Getting the IntersectionObserver logic right for triggering section reveals cleanly took iteration. The ANC bar suppression animation was the most satisfying detail to get working.

---

## About

Built by Youbo (Damon) Bao, a student developer at Ridley College interested in mechanical engineering, aerospace, and building things at the intersection of physics and software.
