---
name: Solo Authority
colors:
  surface: '#101415'
  surface-dim: '#101415'
  surface-bright: '#363a3b'
  surface-container-lowest: '#0b0f10'
  surface-container-low: '#191c1e'
  surface-container: '#1d2022'
  surface-container-high: '#272a2c'
  surface-container-highest: '#323537'
  on-surface: '#e0e3e5'
  on-surface-variant: '#c6c6ca'
  inverse-surface: '#e0e3e5'
  inverse-on-surface: '#2d3133'
  outline: '#8f9094'
  outline-variant: '#45474a'
  surface-tint: '#c6c6ca'
  primary: '#c6c6ca'
  on-primary: '#2f3034'
  primary-container: '#121417'
  on-primary-container: '#7d7e82'
  inverse-primary: '#5d5e62'
  secondary: '#b9c7e0'
  on-secondary: '#233144'
  secondary-container: '#3c4a5e'
  on-secondary-container: '#abb9d2'
  tertiary: '#3cddc7'
  on-tertiary: '#003731'
  tertiary-container: '#001814'
  on-tertiary-container: '#008e7f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e6'
  primary-fixed-dim: '#c6c6ca'
  on-primary-fixed: '#1a1c1f'
  on-primary-fixed-variant: '#45474a'
  secondary-fixed: '#d5e3fd'
  secondary-fixed-dim: '#b9c7e0'
  on-secondary-fixed: '#0d1c2f'
  on-secondary-fixed-variant: '#3a485c'
  tertiary-fixed: '#62fae3'
  tertiary-fixed-dim: '#3cddc7'
  on-tertiary-fixed: '#00201c'
  on-tertiary-fixed-variant: '#005047'
  background: '#101415'
  on-background: '#e0e3e5'
  surface-variant: '#323537'
typography:
  headline-xl:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  label-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 48px
  stack-xl: 80px
---

## Brand & Style

The brand personality is defined by "The Expert Individual"—a synthesis of high-level corporate professionalism and the agile, personal touch of a solo founder. This design system utilizes a **Minimalist-Modern** aesthetic that prioritizes content over container. By stripping away unnecessary ornamentation, the UI signals confidence and clarity, suggesting that the user's time is respected and the founder's output is precise.

The emotional response should be one of quiet reliability. The use of generous whitespace is not merely an aesthetic choice but a functional one, providing "breathing room" that prevents information density from becoming overwhelming. The visual language is intentional, using subtle transitions and a constrained palette to create a high-end, bespoke feel.

## Colors

This design system employs a "Deep Slate" dark mode as its default state to evoke a premium, editorial feel. The palette is anchored by **Deep Charcoal** (#121417) for the primary background, providing a sophisticated alternative to pure black. 

**Slate Grey** (#334155) serves as the secondary color, used for UI borders and secondary surfaces to create soft depth. The accent color, **Forest Teal** (#2DD4BF), is used sparingly—only for primary calls to action, active states, and critical progress indicators—to ensure it retains its visual impact. Text is rendered in **Off-White** (#F8FAFC) to reduce eye strain while maintaining high readability against the dark backdrop.

## Typography

**Manrope** is selected as the sole typeface for its geometric precision and modern, balanced proportions. It bridges the gap between technical utility and approachable elegance. 

Headlines utilize tighter tracking and heavier weights to establish a strong visual hierarchy. Body text is optimized for legibility with a generous 1.6x line-height. Labels and small utility text should be set in uppercase with increased letter spacing to provide a "metadata" feel that distinguishes functional text from narrative content.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** model for desktop to ensure content remains centered and focused, reflecting the singular vision of a solo founder. On mobile, the system shifts to a fluid model with a 4-column structure.

Whitespace is used as a structural element. Sections are separated by large vertical gaps (stack-xl) to emphasize the transition between ideas. Content is often set in a single-column layout or a 60/40 split to maintain a clear reading path. The 8px base unit ensures mathematical consistency across all margins, paddings, and component dimensions.

## Elevation & Depth

Depth in this design system is achieved through **Tonal Layers** rather than heavy shadows. In a dark environment, elevation is communicated by increasing the lightness of the surface color.

1.  **Base Layer:** The Deep Charcoal background.
2.  **Surface Layer:** A slightly lighter charcoal (#1E2126) for cards and sections.
3.  **Overlay Layer:** A slate-grey tint for modals and floating menus.

To maintain a crisp, professional look, use **Low-Contrast Outlines** (1px solid #334155) on all containers. This replaces the need for drop shadows, keeping the UI flat yet structured. A very subtle, 15% opacity ambient glow using the accent color can be applied to the primary CTA to give it a "lift" without breaking the minimalist aesthetic.

## Shapes

The shape language is **Soft** (4px/0.25rem radius). This subtle rounding takes the edge off the "brutal" minimalist aesthetic, making the interface feel more personal and engineered. It strikes a balance between the clinical feel of sharp corners and the overly playful nature of high-radius circles.

Buttons and input fields should strictly follow the `rounded` (4px) or `rounded-lg` (8px) values. Icons should be stroke-based with a 1.5px or 2px weight and slightly rounded caps to match the component geometry.

## Components

### Buttons
Primary buttons use the Forest Teal accent with black text for maximum contrast. Secondary buttons use a slate border with off-white text. Buttons should have generous horizontal padding (24px) to emphasize their importance.

### Cards
Cards are defined by their 1px slate border and lack of background fill on the base layer, or a subtle tonal shift when placed on a secondary surface. Do not use shadows; rely on the border to define the boundary.

### Input Fields
Inputs are minimal: a bottom-border only in the default state, shifting to a full 1px slate border with a Forest Teal focus ring upon interaction. Labels are always small-cap and positioned above the field.

### Progress & Status
Use the Forest Teal accent for progress bars and "active" status chips. Status chips should be small, with a subtle background tint (10% opacity of the accent color) and a 1px solid border of the accent color.

### Navigation
The navigation should be sparse. Use a top-aligned bar with text-only links. The "Home" or "Logo" element should be typographic rather than a complex mark, reinforcing the personal-professional narrative.