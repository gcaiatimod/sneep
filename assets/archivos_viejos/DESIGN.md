---
name: Poncho Digital Standard
colors:
  surface: '#fbf9f8'
  surface-dim: '#dcd9d9'
  surface-bright: '#fbf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f0eded'
  surface-container-high: '#eae8e7'
  surface-container-highest: '#e4e2e1'
  on-surface: '#1b1c1c'
  on-surface-variant: '#404751'
  inverse-surface: '#303030'
  inverse-on-surface: '#f3f0f0'
  outline: '#717882'
  outline-variant: '#c0c7d2'
  surface-tint: '#0062a1'
  primary: '#005994'
  on-primary: '#ffffff'
  primary-container: '#0072bb'
  on-primary-container: '#ebf2ff'
  inverse-primary: '#9ccaff'
  secondary: '#1b6d24'
  on-secondary: '#ffffff'
  secondary-container: '#a0f399'
  on-secondary-container: '#217128'
  tertiary: '#784d00'
  on-tertiary: '#ffffff'
  tertiary-container: '#996300'
  on-tertiary-container: '#fff0e2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d0e4ff'
  primary-fixed-dim: '#9ccaff'
  on-primary-fixed: '#001d35'
  on-primary-fixed-variant: '#00497b'
  secondary-fixed: '#a3f69c'
  secondary-fixed-dim: '#88d982'
  on-secondary-fixed: '#002204'
  on-secondary-fixed-variant: '#005312'
  tertiary-fixed: '#ffddb5'
  tertiary-fixed-dim: '#ffb957'
  on-tertiary-fixed: '#2a1800'
  on-tertiary-fixed-variant: '#643f00'
  background: '#fbf9f8'
  on-background: '#1b1c1c'
  surface-variant: '#e4e2e1'
typography:
  display-metric:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Noto Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Noto Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Noto Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1200px
  gutter: 1.5rem
  margin-mobile: 1rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
  stack-lg: 3rem
---

## Brand & Style
This design system is built upon the principles of institutional clarity, accessibility, and democratic transparency, following the digital standards of the Argentine Government. The brand personality is authoritative yet approachable, prioritizing the efficient delivery of public information over decorative flair.

The design style is **Corporate / Modern** with a specific emphasis on **Data Hierarchy**. It utilizes a "Clean-Official" aesthetic characterized by high legibility, generous whitespace, and structured information density. The emotional response should be one of reliability and civic trust, ensuring that citizens feel the platform is a stable, official source of truth.

## Colors
The palette is dominated by "Azul Poncho" (#0072BB), which serves as the primary anchor for all interactive elements and institutional headers. 

- **Primary**: Used for buttons, active states, and the distinct 5px top borders on priority cards.
- **Secondary/Tertiary**: Reserved for semantic data visualization (e.g., positive/negative trends in sparklines) and categorization of different "Series de Tiempo".
- **Neutral**: A range of grays ensures high contrast ratios for text (WCAG AA/AAA compliance). Surfaces are predominantly white (#FFFFFF) or very light gray (#F9F9F9) to maintain a clean, official look.

## Typography
The typography system uses **Hanken Grotesk** (as a contemporary high-quality alternative to Encode Sans) for headlines and metrics to provide a sharp, geometric authority. **Noto Sans** is used for all body copy and labels to ensure maximum cross-platform compatibility and legibility.

- **Metrics**: Large numerical data in "Series de Tiempo" cards use the `display-metric` style to ensure immediate impact.
- **Hierarchy**: Use `label-caps` for overlines and category tags. 
- **Scale**: On mobile devices, headline sizes scale down to prevent awkward line breaks while maintaining the 5px border-to-headline proportional relationship.

## Layout & Spacing
The system utilizes a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

- **Series de Tiempo Cards**: These typically span 4 columns on desktop (3 per row) or 6 columns (2 per row) depending on the dashboard density.
- **Rhythm**: Vertical spacing follows a strict 8px baseline power-of-two scale. 
- **Margins**: A 24px (1.5rem) gutter is maintained between cards to allow the white surfaces to breathe against light gray backgrounds.

## Elevation & Depth
This design system avoids heavy shadows to maintain a flat, official aesthetic. 

- **Surface Tiers**: Depth is communicated through **Low-contrast outlines** (#E6E6E6) and background tinting.
- **Card Shadows**: Use a single, very subtle ambient shadow (0px 2px 4px rgba(0,0,0,0.05)) to lift cards slightly from the background.
- **Interaction**: On hover, cards do not lift; instead, the 5px top border may increase slightly in vibrance or the background may subtlely shift to a "hover" gray state.

## Shapes
The shape language is **Soft (0.25rem)**. This provides a professional balance—sharp enough to feel institutional and serious, but with slight rounding to feel modern and digitally native. 

- **Cards**: Use 4px corner radius.
- **Buttons**: Use 4px corner radius.
- **Top Border**: The 5px colored accent on cards must remain square-edged at the top to emphasize the structural "line" of the data series.

## Components

### Series de Tiempo Cards
The signature component of this design system.
- **Structure**: A white container with a 4px corner radius and a 1px light gray border.
- **Header**: A 5px thick solid top border using the primary or semantic category color.
- **Content**: Vertical stack including: Category Label (Caps), Main Metric (Large), and a Sparkline Chart.
- **Sparkline**: A simplified line chart without axes, positioned at the bottom of the card content area, showing the trend over time.

### Buttons
- **Primary**: Solid #0072BB background with white text. No gradients.
- **Outline**: 2px border in primary color with transparent background.

### Inputs & Form Fields
- **Style**: Rectangular with a 1px neutral-300 border. Focus state uses a 2px #0072BB outline with a light blue glow.
- **Labels**: Always positioned above the field, never as placeholder text only.

### Lists & Tables
- **Data Tables**: Minimalist approach with horizontal separators only. Header row should have a light gray background (#F3F3F3) to distinguish from data rows.