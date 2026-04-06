# Design System — rsingla.ca

## Product Context
- **What this is:** Personal academic portfolio website for Rohit Singla
- **Who it's for:** Academic peers, potential collaborators, hiring/review committees, biotech investors
- **Space/industry:** Academic medicine, biomedical engineering, medical AI
- **Project type:** Personal academic website (static, GitHub Pages)

## Aesthetic Direction
- **Direction:** Editorial/Refined
- **Decoration level:** Intentional — texture through typography contrast (serif headlines vs sans body), not decorative elements
- **Mood:** Confident, considered, credible. A clinician-engineer who cares about craft. Not a Bootstrap template, not a flashy portfolio. Content-first with quiet sophistication.
- **Anti-patterns:** No icons in colored circles, no gradient hero banners, no purple gradients, no 3-column feature grids, no centered everything

## Typography
- **Display/Hero:** Instrument Serif — contemporary serif with personality, sets the site apart from generic sans-serif academic sites instantly
- **Body:** Source Sans 3 — designed for long-form readability, excellent for publication titles and bio text, supports tabular figures
- **UI/Labels:** Source Sans 3 (same as body, weight 600)
- **Data/Tables:** Source Sans 3 with tabular-nums feature
- **Code:** JetBrains Mono
- **Loading:** Google Fonts CDN
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Instrument+Serif&family=Source+Sans+3:ital,wght@0,300;0,400;0,600;0,700;1,400&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
  ```
- **Scale:**
  - Display: 48px / 3rem
  - H1: 35px / 2.2rem
  - H2: 26px / 1.6rem
  - H3: 17px / 1.05rem (bold, sans-serif)
  - Body: 17px / 1rem
  - Small: 15px / 0.92rem
  - Caption: 13px / 0.82rem (mono)

## Color
- **Approach:** Restrained — one accent + neutrals, color is rare and meaningful
- **Background:** #FAFAF8 — warm off-white, not clinical gray
- **Surface:** #FFFFFF — cards, elevated elements
- **Primary text:** #1A1A2E — deep navy-black with more depth than pure black
- **Muted text:** #6B7280
- **Accent:** #2563EB — confident blue, nods to medical imaging
- **Accent hover:** #1D4ED8
- **Border:** #E5E7EB
- **Header/Footer bg:** #1A1A2E
- **Header/Footer text:** #E5E7EB
- **Semantic:** success #22C55E, warning #F59E0B, error #EF4444, info #2563EB
- **Dark mode strategy:**
  - Background: #0F0F1A
  - Surface: #1A1A2E
  - Primary text: #E5E7EB
  - Muted text: #9CA3AF
  - Accent: #60A5FA (lighter blue for dark backgrounds)
  - Border: #2D2D44

## Spacing
- **Base unit:** 8px
- **Density:** Comfortable — generous spacing signals confidence
- **Scale:** 2xs(2px) xs(4px) sm(8px) md(16px) lg(24px) xl(32px) 2xl(48px) 3xl(64px)

## Layout
- **Approach:** Grid-disciplined with asymmetric profile section
- **Grid:** Sidebar (280px) + fluid content column, single column on mobile (<900px)
- **Max content width:** 960px
- **Border radius:** sm:4px, md:8px, lg:12px

## Motion
- **Approach:** Minimal-functional
- **Easing:** enter(ease-out) exit(ease-in) move(ease-in-out)
- **Duration:** micro(50-100ms) short(150-250ms) medium(250-400ms)
- **Usage:** Link hover color transitions, smooth scrolling. No entrance animations. Academic credibility and flashy animations don't mix.

## Decisions Log
| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-04-01 | Initial design system created | Created by /design-consultation. Editorial/Refined aesthetic with Instrument Serif + Source Sans 3. Professional with personality — credible for academic audience while visually distinctive. |
| 2026-04-01 | Instrument Serif for display | Risk: breaks from sans-serif-everything norm in academic sites. Gain: instant memorability and taste signal. |
| 2026-04-01 | Warm off-white background #FAFAF8 | Risk: minimal. Gain: avoids sterile gray/white of typical academic sites, feels intentional. |
