---
name: Kinetic Trust
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#0b1c30'
  on-tertiary-container: '#75859d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#d3e4fe'
  tertiary-fixed-dim: '#b7c8e1'
  on-tertiary-fixed: '#0b1c30'
  on-tertiary-fixed-variant: '#38485d'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1280px
  auth-card-width: 440px
  gutter: 1.5rem
  stack-sm: 0.5rem
  stack-md: 1rem
  stack-lg: 2rem
---

## Brand & Style

The design system is engineered for high-stakes professional environments where security and clarity are paramount. It targets enterprise users, developers, and financial professionals who require an interface that feels both robust and frictionless. 

The aesthetic is **Corporate Modern**, characterized by a rigorous adherence to grid systems, purposeful whitespace, and a high-fidelity finish. It avoids unnecessary ornamentation, focusing instead on "functional elegance"—where the quality of the interface is communicated through precise alignment, balanced proportions, and a sophisticated color logic. The goal is to evoke a sense of stability, technological maturity, and institutional reliability.

## Colors

The palette is anchored by "Slate 950" (#0F172A), a deep, authoritative blue-black used for primary branding and headings to establish immediate gravitas. The primary action color is a vibrant "Blue 600" (#3B82F6), selected for its high visibility and association with trust and digital-first services.

- **Primary:** Deep Slate. Used for core brand elements, high-contrast text, and primary navigation.
- **Accent:** Electric Blue. Reserved for primary calls-to-action, active states, and focus indicators.
- **Surface:** A range of cool grays (Slate 50 to 200). Used to create subtle separation between UI regions without relying on heavy borders.
- **Status:** Standard semantic colors for Error (#EF4444), Success (#10B981), and Warning (#F59E0B) should be desaturated slightly to match the professional tone.

## Typography

This design system utilizes **Inter** exclusively. It is a systematic, utilitarian typeface designed for screens, offering exceptional legibility at small sizes and a clean, technical appearance in display settings.

The type hierarchy is strictly enforced. Headlines use tighter letter-spacing and heavier weights to project confidence. Body text utilizes "Slate 600" for secondary information and "Slate 900" for primary content to ensure optimal reading contrast. Labels and small metadata should use `label-sm` with slight tracking (0.02em) to maintain readability in condensed UI areas.

## Layout & Spacing

The layout follows a **Fixed-Width Centered** model for authentication flows, transitioning to a **Fluid Grid** for internal dashboards. 

- **Authentication Layout:** Content is contained within a 440px central card. This limitation reduces eye strain and creates a focused, secure-feeling environment.
- **Grid:** A 12-column grid is used for the underlying structure.
- **Rhythm:** An 8px linear scale (0.5rem) governs all spacing. Vertical stacks between form elements should be 24px (`1.5rem`), while the spacing between a label and its input is a tight 8px (`0.5rem`).
- **Responsive:** On mobile devices, margins shrink to 16px, and the central card expands to fill the screen width with a simplified header.

## Elevation & Depth

Hierarchy is achieved through **Tonal Layering** and **Minimal Ambient Shadows**. 

The base background uses `Slate 50`. Primary cards and containers use a pure white (`#FFFFFF`) background with a very subtle 1px border (`Slate 200`). Elevation is indicated by a soft, multi-layered shadow:
- **Low Elevation (Inputs/Buttons):** A slight 1px Y-offset shadow with 5% opacity to give a "lifted" feel from the page.
- **Medium Elevation (Modals/Cards):** A diffused 12px blur shadow with 8% opacity.

Avoid heavy dark shadows; the "depth" should feel like light catching the edge of a physical object rather than a floating element.

## Shapes

The shape language is **Soft** and disciplined. A corner radius of `0.25rem` (4px) is the standard for most components, including input fields and buttons. This creates a professional look that is approachable but remains "square" enough to feel architectural and serious. 

Larger containers like authentication cards may use `rounded-lg` (8px) to provide a slightly softer frame for the entire interaction.

## Components

### Input Fields
Inputs are the core of the authentication experience. Use a `Slate 300` border by default. On focus, the border transitions to `Blue 600` with a 3px outer "glow" (a semi-transparent blue ring) to signify the active state. Labels must be positioned above the field, never as placeholders only.

### Buttons
- **Primary:** Solid `Slate 950` or `Blue 600` background with white text. Use a subtle hover state that darkens the color by 10%.
- **Social Login:** Use a white background with a 1px `Slate 200` border. Icons should be centered with a small gap before the text.

### Chips & Badges
Used for indicating status or multi-factor settings. These should be "flat"—no shadows—using a light tinted background (e.g., `Blue 50`) and a darker text color (e.g., `Blue 700`).

### Checkboxes
Small, 16px square boxes with `rounded-sm` corners. When checked, they should fill with the Primary color and show a crisp white checkmark.

### Progress Indicators
For multi-step authentication, use a thin, 4px horizontal bar at the top of the container. Completed segments should be `Blue 600`, while remaining segments are `Slate 200`.