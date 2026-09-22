---
name: Kinetic Noir
colors:
  surface: '#1d100a'
  surface-dim: '#1d100a'
  surface-bright: '#46362e'
  surface-container-lowest: '#170b06'
  surface-container-low: '#261812'
  surface-container: '#2b1c16'
  surface-container-high: '#362720'
  surface-container-highest: '#41312a'
  on-surface: '#f8ddd2'
  on-surface-variant: '#e2bfb0'
  inverse-surface: '#f8ddd2'
  inverse-on-surface: '#3d2d26'
  outline: '#a98a7d'
  outline-variant: '#5a4136'
  surface-tint: '#ffb693'
  primary: '#ffb693'
  on-primary: '#561f00'
  primary-container: '#ff6b00'
  on-primary-container: '#572000'
  inverse-primary: '#a04100'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#9ccaff'
  on-tertiary: '#003257'
  tertiary-container: '#059eff'
  on-tertiary-container: '#003357'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbcc'
  primary-fixed-dim: '#ffb693'
  on-primary-fixed: '#351000'
  on-primary-fixed-variant: '#7a3000'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#d0e4ff'
  tertiary-fixed-dim: '#9ccaff'
  on-tertiary-fixed: '#001d35'
  on-tertiary-fixed-variant: '#00497b'
  background: '#1d100a'
  on-background: '#f8ddd2'
  surface-variant: '#41312a'
typography:
  display-hero:
    fontFamily: sora
    fontSize: 120px
    fontWeight: '800'
    lineHeight: 110px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: sora
    fontSize: 64px
    fontWeight: '700'
    lineHeight: 72px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: sora
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: sora
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: jetbrainsMono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.15em
spacing:
  unit: 8px
  container-max: 1440px
  gutter: 32px
  margin-desktop: 80px
  margin-mobile: 20px
  section-gap: 160px
---

## Brand & Style

The design system embodies a **Cinematic Architectural** style. It is defined by a rigorous commitment to darkness, utilizing "void-space" rather than just whitespace to create a sense of infinite depth. The aesthetic is inspired by high-end automotive configurators and premium architectural portfolios—where lighting is the primary tool for defining form.

The mood is **authoritative and vanguard**. It avoids the clutter of traditional SaaS interfaces in favor of a curated, studio-grade environment. Visual interest is generated through high-contrast typography and "atmospheric light leaks" that mimic the orange glow of the reference logo's core. 

Key principles:
- **Optical Precision:** Every element is aligned to a strict geometric grid.
- **Luminance over Color:** Surfaces are defined by their reflectivity and interaction with light rather than flat fills.
- **Architectural Scale:** Dramatic shifts in typography scale create a sense of physical grandeur.

## Colors

The palette is anchored in **Absolute Zero (#050505)** to ensure the deepest possible blacks on OLED screens, providing a canvas where light can truly pop. 

- **Primary (Core Orange):** Used exclusively for high-intent actions, critical data points, and "light-glow" effects. It represents the energy and results of the agency.
- **Surface Tiers:** Use a palette of deep charcoals. Borders should use low-opacity white (5-10%) to create "shimmer" edges rather than solid lines.
- **Typography:** Pure white (#FFFFFF) for headlines to ensure maximum "punch" against the dark background. Body text is softened to a high-density grey to maintain long-form readability without visual vibration.

## Typography

The typographic system uses **Sora** for headlines to achieve a geometric, technical, yet premium feel. The tracking is tightened in large sizes to create a dense, "block-like" architectural presence. 

- **Display Hierarchy:** The `display-hero` style is intended for oversized branding moments, often overlapping with 3D elements or imagery.
- **Monospaced Accents:** **JetBrains Mono** is utilized for metadata, labels, and technical callouts, reinforcing the "digital studio" and precision-engineered personality.
- **Contrast:** Always maintain a high contrast ratio. Headlines should be pure white, while body copy is slightly muted to reduce eye strain in the dark environment.

## Layout & Spacing

This design system utilizes a **12-column fixed-center grid** for desktop and a **4-column fluid grid** for mobile. 

The layout philosophy is defined by **Macro-Spacing**. We use aggressive vertical padding (Section Gaps) to isolate content blocks, forcing the user to focus on one "scene" at a time, much like a film reel.

- **Asymmetry:** Leverage the 12-column grid to create asymmetrical layouts (e.g., content spanning columns 2-7, with metadata in column 9).
- **Safe Areas:** Maintain generous margins (80px+) to prevent the interface from feeling "cramped" or standard-issue.
- **Reflow:** On mobile, verticality is emphasized. Stack all elements and increase the tracking on `label-caps` for better legibility on small screens.

## Elevation & Depth

Depth is not communicated via shadows, but through **Luminance and Refraction**.

- **Glassmorphism:** Use semi-transparent surfaces for overlays and navigation bars. Apply a `backdrop-filter: blur(20px)` and a subtle `1px` white border at 10% opacity on the top and left edges to simulate light hitting a glass edge.
- **Atmospheric Glows:** Use large, low-opacity radial gradients of the Primary Orange (#FF6B00) behind key elements to create a sense of "lighting" within a 3D space.
- **Z-Axis Layers:** 
  1. **Level 0 (Base):** #050505.
  2. **Level 1 (Cards):** #0F0F0F with a 1px stroke.
  3. **Level 2 (Modals/Popovers):** Glass-blurred surfaces that "float" over the content.

## Shapes

The design system utilizes **Sharp (0px)** roundedness. 

The 3D logo's cubic, monolithic structure dictates a visual language of hard edges and right angles. This reinforces the "Architectural" pillar of the brand. Every button, input field, and card must be perfectly rectangular. 

The only exception to the "square" rule is the use of circular "light halos" in the background, which act as a soft organic foil to the rigid structural elements.

## Components

### Buttons
- **Primary:** Sharp-edged rectangle. Background is #FF6B00. Text is Black (#050505) for maximum contrast. On hover, the button should emit a soft orange outer glow.
- **Secondary:** Transparent background with a 1px white border (30% opacity). White text. On hover, the border becomes 100% white.

### Input Fields
- Underline style only, or a fully enclosed box with #0F0F0F fill. No rounded corners. Focus state is indicated by the bottom border changing to Primary Orange with a subtle "neon" glow.

### Cards
- Use a "Glass-Dark" style: Background #0F0F0F at 80% opacity with backdrop-blur. The top border should be slightly brighter than the side borders to simulate overhead studio lighting.

### Navigation
- A floating "Glass" bar at the top or bottom of the viewport. Use high-contrast white text for links. Active states should be marked by a small 4x4px orange square (a "pixel") rather than a standard underline.

### Chips/Tags
- Small, monospaced text (JetBrains Mono) inside a sharp-edged box with a subtle grey border. No fill. Used for categorizing technical capabilities or project sectors.