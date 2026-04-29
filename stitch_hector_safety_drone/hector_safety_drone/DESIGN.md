---
name: HECTOR Safety Drone
colors:
  surface: '#10131b'
  surface-dim: '#10131b'
  surface-bright: '#363942'
  surface-container-lowest: '#0b0e16'
  surface-container-low: '#181c23'
  surface-container: '#1c2027'
  surface-container-high: '#272a32'
  surface-container-highest: '#31353d'
  on-surface: '#e0e2ed'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#e0e2ed'
  inverse-on-surface: '#2d3039'
  outline: '#8b90a0'
  outline-variant: '#414754'
  surface-tint: '#adc7ff'
  primary: '#adc7ff'
  on-primary: '#002e68'
  primary-container: '#4a8eff'
  on-primary-container: '#00285b'
  inverse-primary: '#005bc0'
  secondary: '#b9c7e4'
  on-secondary: '#233148'
  secondary-container: '#3c4962'
  on-secondary-container: '#abb9d6'
  tertiary: '#b6c6ed'
  on-tertiary: '#20304f'
  tertiary-container: '#8191b5'
  on-tertiary-container: '#192948'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc7ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#d6e3ff'
  secondary-fixed-dim: '#b9c7e4'
  on-secondary-fixed: '#0d1c32'
  on-secondary-fixed-variant: '#39475f'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#b6c6ed'
  on-tertiary-fixed: '#091b39'
  on-tertiary-fixed-variant: '#374767'
  background: '#10131b'
  on-background: '#e0e2ed'
  surface-variant: '#31353d'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.01em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  gutter: 24px
  margin: 32px
  card-padding: 24px
  container-max-width: 1440px
---

## Brand & Style

The design system is engineered to project an image of absolute reliability, technical precision, and authoritative security. It is designed for high-stakes environments where clarity and rapid data processing are paramount. The aesthetic targets a "Mission Control" feel—sophisticated but accessible.

The visual direction utilizes **Glassmorphism** combined with **Modern Corporate** layouts. By layering translucent surfaces over a deep, atmospheric background, the interface achieves a sense of depth and high-tech sophistication. This style emphasizes "augmented reality" qualities, suggesting that the data is floating over a digital landscape, reinforcing the drone-centric nature of the product. The overall emotional response should be one of calm confidence and cutting-edge capability.

## Colors

The palette is anchored by a **Deep Navy (#0A192F)** background to reduce eye strain during extended monitoring and to provide a premium, nighttime-operational feel. The **Safety Blue (#007BFF)** acts as the primary action color, providing a high-contrast focal point that signifies technology and trust.

A secondary navy tier (#112240) is used for card backgrounds and container fills. Safety is communicated through a strictly enforced semantic system:
- **Green (#28C76F):** Optimal safety scores and operational readiness.
- **Yellow (#FF9F43):** Cautionary alerts or mid-range safety fluctuations.
- **Red (#EA5455):** Immediate threats or system failures.

Borders on glass elements use a low-opacity white (10-15%) to define edges without breaking the translucent effect.

## Typography

The design system utilizes **Inter** for its exceptional legibility and systematic, utilitarian appearance. The type hierarchy is structured to support rapid scanning of telemetry and safety data.

- **Headlines:** Use tighter letter spacing and bold weights to command authority.
- **Labels:** Small caps with increased tracking (letter spacing) are used for technical metadata and drone identifiers, mimicking aerospace readouts.
- **Data Display:** Numerical values should utilize a medium weight to ensure they stand out against descriptive text labels.

## Layout & Spacing

The layout follows a **Fluid Grid** model optimized for a professional dashboard environment. It uses a 12-column system that adapts to various screen sizes while maintaining consistent 24px gutters.

Spacing is based on an **8px linear scale**. High-priority telemetry modules typically span 4 or 6 columns, while secondary status feeds utilize 3-column slots. The generous 32px outer margins ensure the UI feels expansive and "de-cluttered," which is essential for maintaining operator focus during critical safety events.

## Elevation & Depth

This design system avoids traditional drop shadows in favor of **Tonal Layering and Glassmorphism**. Depth is established through the following hierarchy:

1.  **Level 0 (Base):** Deep Navy (#0A192F) solid background.
2.  **Level 1 (Cards):** Translucent fill (White @ 5% opacity) with a 20px Backdrop Blur. Edges are defined by a 1px "Inner Glow" border (White @ 10%).
3.  **Level 2 (Modals/Popovers):** Higher opacity fill (White @ 10%) with a 40px Backdrop Blur and a subtle 16px ambient shadow tinted with the Primary Blue to simulate a glow effect.

Visual separation is achieved through color contrast and blur intensity rather than heavy black shadows.

## Shapes

The shape language is defined by large, sophisticated radii that soften the high-tech aesthetic, making the advanced technology feel approachable and modern.

- **Primary Containers:** 16px (rounded-lg) for main dashboard cards and modules.
- **Buttons & Inputs:** 8px (rounded-md) to provide a precise, clickable appearance.
- **Status Pills:** Fully rounded (pill-shaped) to distinguish them from structural UI elements.

The consistent use of rounded corners (16px+) across all major containers is a core signature of the design system, ensuring a cohesive "capsule" look for all data points.

## Components

### Buttons
Primary buttons use a solid Safety Blue (#007BFF) fill with white text. Secondary buttons use a glass background with a blue border. States (Hover/Active) should be indicated by a subtle increase in glow or brightness, rather than a color shift to a different hue.

### Glass Cards
The cornerstone component. Every card must include a `backdrop-filter: blur(20px)` and a `border: 1px solid rgba(255,255,255,0.1)`. Padding is strictly 24px to maintain an airy, premium feel.

### Status Indicators
Status scores are displayed as large, circular gauges or high-contrast chips. The color mapping (Green/Yellow/Red) must be the most prominent feature of these components.

### Input Fields
Inputs are dark-themed with a subtle 5% white fill. On focus, the border transitions to Safety Blue with a 4px outer glow of the same color.

### Drone Telemetry Lists
Lists utilize alternating row opacities (3% vs 0%) instead of solid lines to separate data, maintaining the clean, glass-like aesthetic without adding visual noise.