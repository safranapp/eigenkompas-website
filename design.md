---
version: alpha
name: Eigenkompas.design
description: Warm nature-editorial design system — cream paper, forest-green primary with mint highlight, navy depth, warm brown, Cormorant Garamond + Jost, sharp corners, hairline borders, generous negative space.
colors:
  primary: "#2E5B40"
  primary-light: "#3D7454"
  on-primary: "#FFFFFF"
  mint: "#6EC68A"
  navy: "#1B2D4F"
  brown: "#8B7251"
  background: "#FAFAF8"
  surface: "#F5F1EB"
  white: "#FFFFFF"
  text-primary: "#1A1A2E"
  text-secondary: "#6B7280"
  on-dark: "#FFFFFF"
  border: "#E5E0D8"
  border-on-dark: "rgba(255,255,255,0.10)"
typography:
  display: { fontFamily: "Cormorant Garamond", fontSize: 96px, fontWeight: 300, lineHeight: 0.95, letterSpacing: -0.01em }
  heading: { fontFamily: "Cormorant Garamond", fontSize: 48px, fontWeight: 300, lineHeight: 1.1 }
  stat: { fontFamily: "Cormorant Garamond", fontSize: 60px, fontWeight: 300, lineHeight: 1 }
  body-lg: { fontFamily: Jost, fontSize: 18px, fontWeight: 300, lineHeight: 1.9 }
  body-md: { fontFamily: Jost, fontSize: 15px, fontWeight: 300, lineHeight: 1.9 }
  eyebrow: { fontFamily: Jost, fontSize: 12px, fontWeight: 400, letterSpacing: 0.28em, textTransform: uppercase }
  label: { fontFamily: Jost, fontSize: 12px, fontWeight: 400, letterSpacing: 0.2em, textTransform: uppercase }
rounded: { none: 0px, blob: "60%", pill: 9999px }
spacing: { xs: 4px, sm: 8px, md: 16px, lg: 24px, xl: 40px, section: 96px }
components:
  button-primary: { backgroundColor: "{colors.primary}", textColor: "{colors.on-primary}", border: "1px solid {colors.primary}", rounded: "{rounded.none}", padding: "20px 36px", font: "{typography.label}" }
  button-outline: { backgroundColor: transparent, textColor: "{colors.text-primary}", border: "1px solid {colors.primary}", rounded: "{rounded.none}", padding: "20px 36px", font: "{typography.label}" }
  card: { backgroundColor: "{colors.white}", border: "1px solid {colors.border}", rounded: "{rounded.none}", padding: 48px }
  eyebrow-label: { color: "{colors.primary}", font: "{typography.eyebrow}" }
---
## Overview
Warm, editorial, grounded, premium. A sheet of warm cream paper, near-black ink, and a disciplined nature accent set — forest green leading, deep navy for depth, warm brown for warmth, mint as a bright highlight on dark surfaces. Character comes from the Cormorant Garamond (serif, light) + Jost (sans, light, wide-tracked) pairing and from italic serif accent words in green inside otherwise plain headlines. Structure comes from sharp-cornered cards separated by hairline borders on a grid. Grounded boutique studio, not stock SaaS. Palette sourced from the live Eigenkompas brand.
## Colors
`background` warm near-white sits under everything; `surface` cream alternates between sections and fills hover/inset cells; `white` lifts crisp cards off cream. `text-primary` is all type; muted text is `text-secondary`. `primary` forest green is the dominant accent — italic emphasis words, primary CTA, stat numerals, eyebrows, card hover fills. `navy` is the dark chapter-section surface and feature-card gradient partner (`green → navy`). `mint` is a bright highlight reserved for dark surfaces only (labels, icons). `brown` is a scarce tertiary warmth (tints, blob). Every light edge is the `border` hairline; on dark, white at 10%.
## Typography
Two families, strict roles. Cormorant Garamond (300–400) for all display, headings, stat numerals, and italic pull-quotes — large, tight leading, slight negative tracking, one italic green accent word per headline. Jost (300) for body (loose 1.9 line-height) and, at 12px UPPERCASE with wide tracking, for eyebrows, nav, buttons, captions, and fine print. If it's big it's serif; if it's small and uppercase it's Jost. Body is never set in the serif.
## Layout
`max-w-7xl` container, sections at 96px vertical / 64px horizontal padding, alternating `background` ↔ `surface`, separated by hairline `border-y`. Signature pattern: cards in a `gap-px` grid over a border-colored background so gaps read as dividers. Common grids: 3-up services, 2-up portfolio with an occasional double-width feature tile, 4-up stat bar. Hero is two-column (headline left, tall `green → navy` feature card right) with a soft brown/cream blob bleeding off the top-right behind it. One navy section per page acts as a dark chapter break. Collapses to single column on mobile.
## Elevation & Depth
Depth from borders, surface-tone shifts, and color inversion — not shadows. The only shadow is the hero feature card (very low-opacity navy/green). Hover feedback is a 1px `-translate-y` plus fill/text inversion to green, never a shadow bloom.
## Shapes
Sharp corners everywhere (`rounded-none`) — the defining trait. Hairline 1px borders (`#E5E0D8`) define edges. The only curve is the atmospheric hero background blob (`border-radius` 60% on one corner) in soft brown/cream, behind content, holding no UI. No pills, no rounded images.
## Components
Buttons are square: primary = green fill / white text, outline = transparent / ink text; both invert on hover, Jost uppercase `0.2em` tracking, ~20×36px padding. Nav links are uppercase Jost with a left-growing 1px green underline on hover. Every section opens with an eyebrow (uppercase Jost, green; mint on dark) → Cormorant heading with one italic green word → optional Jost lede. Service cards: brown serif numeral → serif heading → body, hover fills green + white + lift. Stat cells: huge green serif numeral over tiny uppercase label. Testimonials sit on the navy section in faint white-fill bordered cards with a giant mint serif quote mark. Portfolio tiles use square aspect-ratio gradient placeholders with an italic serif label and a `border-t` caption. Footer is navy with white text, mint headings. Icons: Iconify solar linear set; never emoji.
## Do's and Don'ts
- Do keep every corner sharp; use hairline borders and `gap-px` grids to divide content.
- Do drop one or two italic Cormorant words in green into plain headlines.
- Do keep green dominant, navy for depth, brown sparing, mint only on dark; set all small text in tracked uppercase Jost; lean on negative space.
- Don't round buttons/cards/inputs/images (hero blob excepted) or use shadows beyond the hero card.
- Don't set body copy in the serif, put mint on cream, let brown compete with green, or use emoji as icons.
