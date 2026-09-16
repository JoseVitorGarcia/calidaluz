---
name: Artisanal Warmth
colors:
  surface: '#fff8f4'
  surface-dim: '#e5d8cc'
  surface-bright: '#fff8f4'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff1e6'
  surface-container: '#faebe0'
  surface-container-high: '#f4e6da'
  surface-container-highest: '#eee0d5'
  on-surface: '#211a14'
  on-surface-variant: '#524436'
  inverse-surface: '#372f28'
  inverse-on-surface: '#fceee3'
  outline: '#857464'
  outline-variant: '#d7c3b0'
  surface-tint: '#875300'
  primary: '#875300'
  on-primary: '#ffffff'
  primary-container: '#d48c2c'
  on-primary-container: '#4b2c00'
  inverse-primary: '#ffb965'
  secondary: '#586244'
  on-secondary: '#ffffff'
  secondary-container: '#dce7c1'
  on-secondary-container: '#5e684a'
  tertiary: '#006689'
  on-tertiary: '#ffffff'
  tertiary-container: '#38a6d7'
  on-tertiary-container: '#00384d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffddba'
  primary-fixed-dim: '#ffb965'
  on-primary-fixed: '#2b1700'
  on-primary-fixed-variant: '#663d00'
  secondary-fixed: '#dce7c1'
  secondary-fixed-dim: '#c0cba7'
  on-secondary-fixed: '#161e07'
  on-secondary-fixed-variant: '#414a2e'
  tertiary-fixed: '#c3e8ff'
  tertiary-fixed-dim: '#79d1ff'
  on-tertiary-fixed: '#001e2c'
  on-tertiary-fixed-variant: '#004c68'
  background: '#fff8f4'
  on-background: '#211a14'
  surface-variant: '#eee0d5'
typography:
  display-lg:
    fontFamily: Libre Caslon Text
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Libre Caslon Text
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Libre Caslon Text
    fontSize: 24px
    fontWeight: '400'
    lineHeight: '1.3'
  body-lg:
    fontFamily: DM Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: DM Sans
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  section-gap: 5rem
  organic-offset: 1.5rem
---

## Brand & Style

The design system is centered on the "Slow Living" movement—an intentional, artisanal approach that prioritizes human touch over mechanical perfection. The brand personality is soulful, warm, and restorative, targeting a conscious consumer who values sustainability and the ritual of home.

The visual style is **Tactile / Organic Minimalism**. It avoids the rigidity of traditional e-commerce by using asymmetrical layouts and hand-drawn flourishes. The emotional response is one of immediate calm, evocative of the soft flicker of a candle and the texture of recycled paper. Elements should feel like they were placed by hand, not snapped to a cold mathematical grid.

## Colors

The palette is derived from natural elements: beeswax, olive groves, and rich soil.

- **Primary (Amber/Honey Gold):** Used for calls to action and focal points, representing the glow of a flame.
- **Secondary (Sage/Olive Green):** Used for sustainability callouts and secondary actions, grounding the brand in nature.
- **Background (Light Cream):** A warm, paper-like canvas that prevents the clinical feel of pure white.
- **Typography (Dark Brown):** A deep, earthy mocha used for all text to ensure high legibility while maintaining a softer contrast than black.

## Typography

This design system uses a pairing of a high-personality serif and a functional sans-serif. **Libre Caslon Text** (serving as a stylistic equivalent to Cormorant Garamond for this context) provides an editorial, literary feel for titles. **DM Sans** is used for body copy to ensure clarity in product descriptions and navigation.

For mobile, `display-lg` should scale down to `32px` to prevent overflow, while maintaining the tight line-height characteristic of artisanal publishing.

## Layout & Spacing

The layout philosophy is **Asymmetrical Fluidity**. While built on a standard 12-column foundation for development ease, visual elements are intentionally offset using "organic-offset" values to break the vertical lines.

- **Generous White Space:** Sections are separated by large vertical gaps to encourage a slow browsing pace.
- **Overlaps:** Images should occasionally overlap background shapes or text blocks to create depth without using traditional shadows.
- **Mobile Behavior:** On mobile, the asymmetry is simplified to a single-column stack, but maintains alternating left/right alignment for text blocks to preserve the brand's "unstructured" rhythm.

## Elevation & Depth

In line with the "Handmade" narrative, this design system eschews digital shadows. Instead, depth is created through **Tonal Layering**:

- **Layer 0:** The main Cream background.
- **Layer 1:** Subtle, organic shapes (blobs or leaf motifs) in a slightly darker "Sand" tint or low-opacity Sage.
- **Layer 2:** Functional cards and containers, which use thin, 1px borders in a muted Amber or Brown rather than shadows.
- **Overlays:** Use very soft, low-opacity background blurs (5px) for navigation menus to mimic the translucency of vellum paper.

## Shapes

The shape language is organic. While buttons use a standard "Rounded" (0.5rem) setting for usability, containers and decorative elements should utilize `border-radius` values that are intentionally inconsistent—for example, a card might have `60% 40% 70% 30% / 40% 50% 60% 40%` to create a "pebble" or "hand-poured" look.

## Components

- **Buttons:** Primary buttons are solid Amber with Dark Brown text. Secondary buttons are outlined in Sage Green with Sage text. All buttons use a soft 8px corner radius.
- **Input Fields:** Use a simple bottom-border only (1px Dark Brown) to maintain a minimal, "notepaper" aesthetic. Labels should be small-caps DM Sans.
- **Cards:** Product cards should not have borders or shadows. Use a slight background tint change on hover and ensure the product photography features natural, soft-focus lighting.
- **Chips/Tags:** Used for sustainability markers (e.g., "Soy Wax"). These should appear as small, pill-shaped elements in low-opacity Sage with dark green text.
- **Dividers:** Use hand-drawn style SVG lines or simple heart/leaf icons (as seen in the reference) to separate content sections instead of horizontal rules.