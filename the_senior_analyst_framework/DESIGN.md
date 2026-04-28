---
name: The Senior Analyst Framework
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8b90a0'
  outline-variant: '#414754'
  surface-tint: '#adc7ff'
  primary: '#adc7ff'
  on-primary: '#002e68'
  primary-container: '#4a8eff'
  on-primary-container: '#00285b'
  inverse-primary: '#005bc0'
  secondary: '#ffb68b'
  on-secondary: '#522300'
  secondary-container: '#ff7f1c'
  on-secondary-container: '#602a00'
  tertiary: '#49e181'
  on-tertiary: '#003919'
  tertiary-container: '#00a756'
  on-tertiary-container: '#003115'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc7ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#ffdbc8'
  secondary-fixed-dim: '#ffb68b'
  on-secondary-fixed: '#321200'
  on-secondary-fixed-variant: '#753400'
  tertiary-fixed: '#6afe9b'
  tertiary-fixed-dim: '#49e181'
  on-tertiary-fixed: '#00210c'
  on-tertiary-fixed-variant: '#005227'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  h1:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: '0'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 40px
  xl: 64px
  gutter: 24px
  margin: 32px
---

## Brand & Style

This design system is built for a high-end data analytics aesthetic, catering to a target audience of C-suite executives and technical stakeholders who value precision, clarity, and strategic insight. The brand personality is authoritative yet modern, characterized by a "SaaS-forward" approach that prioritizes data density without sacrificing legibility.

The visual style is a hybrid of **Minimalism** and **Glassmorphism**. It utilizes clean, systematic layouts typical of professional dashboards, enhanced by subtle translucency and layered surfaces to provide a sense of depth and technical sophistication. The UI should feel like a high-performance instrument panel: calibrated, reliable, and deeply insightful.

## Colors

The palette is anchored in a sophisticated "Deep Slate" hierarchy for backgrounds and containers, ensuring a high-contrast environment that reduces eye strain during prolonged analysis. 

- **Primary (Electric Blue):** Used for core navigation, primary actions, and brand-critical identifiers. It signifies connectivity and intelligence.
- **Secondary (Energetic Orange):** A high-visibility accent reserved for critical call-to-actions, "insight" highlights, or warnings. It should be used sparingly to maintain its impact.
- **Tertiary (Soft Green):** Employed for positive growth metrics, success states, and secondary data visualizations.
- **Neutral (Slate):** Multiple tiers of slate provide the structural foundation for the "dark surface containers," creating clear separation between content zones.

## Typography

This design system exclusively utilizes **Inter** to maintain a neutral, systematic, and utilitarian feel. The typographic scale is optimized for information density. 

Headlines use tighter letter-spacing and heavier weights to command attention, while body text maintains a generous line height for maximum readability against dark backgrounds. Labels and captions are frequently styled with increased letter-spacing and uppercase transformations to distinguish metadata from content, mimicking the look of professional data visualization software.

## Layout & Spacing

The design system employs a **Fixed Grid** model for desktop, centered on a 12-column layout to facilitate complex data arrangements. A strict 4px/8px base-unit scale governs all padding and margins, ensuring mathematical harmony across the interface.

On larger screens, content is contained within a 1280px max-width wrapper. Elements like KPI cards or project snapshots should align with the grid spans (e.g., 3-column span for small metrics, 6-column for charts, 12-column for hero sections). Spacing between cards (gutters) is fixed at 24px to provide enough breathing room for "glassy" surface effects to be visible.

## Elevation & Depth

Depth is conveyed through **Tonal Layers** and **Low-Contrast Outlines**. Rather than aggressive shadows, this design system uses sequential lightening of slate hex codes to indicate "lift."

1.  **Base Layer:** The darkest slate, used for the primary background.
2.  **Surface Containers:** Slightly lighter slate with a 1px border (#334155 at 50% opacity).
3.  **Active/Hover State:** The lightest slate tier, or a subtle backdrop-blur (12px) for a glassmorphic effect.

When shadows are used, they must be "Ambient Shadows"—extremely diffused, large radius (24px-48px), and very low opacity (10-15%), tinted slightly with the primary Electric Blue to feel integrated into the dark environment.

## Shapes

The shape language is "Soft" (Level 1), utilizing a 0.25rem (4px) base radius. This creates a technical, precise appearance that aligns with the "dashboard" aesthetic. 

Higher-level containers like main content cards may use a `rounded-lg` (8px) radius to feel slightly more approachable, but the majority of functional elements—buttons, input fields, and tags—should remain sharp and disciplined. Circles are reserved exclusively for avatars and status indicators to provide a clear geometric contrast to the structural grid.

## Components

- **Buttons:** Primary buttons use a solid Electric Blue fill with white text. Secondary buttons are "Ghost" style: 1px slate borders that transition to a soft blue glow on hover.
- **Cards:** Utilize the "Surface Medium" fill with a subtle 1px top-border to catch a simulated light source. Include "Data Visualization" card types that feature sparklines or mini-bar charts.
- **Chips & Tags:** Small, pill-shaped elements for skills or industry sectors. They use a low-opacity Electric Blue background with high-contrast text.
- **Input Fields:** Darker than the container they sit on, with a subtle 1px border that glows Electric Blue when focused.
- **KPI Modules:** Distinctive components for displaying metrics (e.g., "Project Efficiency: +15%"). Use the Soft Green for positive trends and the Energetic Orange for items requiring attention.
- **Lists:** Clean, border-bottom separated rows with high-contrast headers and muted metadata.