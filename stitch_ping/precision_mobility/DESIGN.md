---
name: Precision Mobility
colors:
  surface: '#fbf9fa'
  surface-dim: '#dbd9db'
  surface-bright: '#fbf9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f4'
  surface-container: '#efedef'
  surface-container-high: '#e9e7e9'
  surface-container-highest: '#e4e2e3'
  on-surface: '#1b1c1d'
  on-surface-variant: '#44474c'
  inverse-surface: '#303032'
  inverse-on-surface: '#f2f0f2'
  outline: '#74777d'
  outline-variant: '#c4c6cd'
  surface-tint: '#4f6073'
  primary: '#041627'
  on-primary: '#ffffff'
  primary-container: '#1a2b3c'
  on-primary-container: '#8192a7'
  inverse-primary: '#b7c8de'
  secondary: '#0058bc'
  on-secondary: '#ffffff'
  secondary-container: '#0070eb'
  on-secondary-container: '#fefcff'
  tertiary: '#211200'
  on-tertiary: '#ffffff'
  tertiary-container: '#38260b'
  on-tertiary-container: '#a88c69'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d2e4fb'
  primary-fixed-dim: '#b7c8de'
  on-primary-fixed: '#0b1d2d'
  on-primary-fixed-variant: '#38485a'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a41'
  on-secondary-fixed-variant: '#004493'
  tertiary-fixed: '#feddb5'
  tertiary-fixed-dim: '#e1c29b'
  on-tertiary-fixed: '#281802'
  on-tertiary-fixed-variant: '#584326'
  background: '#fbf9fa'
  on-background: '#1b1c1d'
  surface-variant: '#e4e2e3'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 30px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 17px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  status-number:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  touch-target-min: 48px
  margin-page: 20px
  gutter-grid: 16px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 24px
  safe-area-bottom: 34px
---

## Brand & Style
The design system is engineered for the high-stakes environment of autonomous vehicle control. The brand personality is authoritative, precise, and reassuringly technical. It prioritizes clarity and immediate cognition over decorative elements.

The aesthetic follows a **Corporate / Modern** direction with a focus on **Minimalism**. It utilizes expansive white space to reduce cognitive load during vehicle operation. High-tech sophistication is conveyed through subtle depth, refined typography, and a strict adherence to a professional color utility system. The interface must feel like a natural extension of the vehicle's internal hardware—reliable and responsive.

## Colors
The palette is dominated by a professional Navy primary and a vibrant Tech Blue secondary used for interactive states and primary actions.

- **Primary (#1A2B3C):** Used for navigation bars, primary headings, and high-importance UI anchors to provide a sense of stability.
- **Secondary (#007AFF):** Reserved for active buttons, links, and selection states.
- **Success (#34C759):** Exclusively for "Online," "Active," and "Safe" vehicle statuses.
- **Danger (#FF3B30):** Reserved for "E-STOP," critical alerts, and immediate intervention triggers.
- **Surface & Background:** A clear distinction is made between the system background (#F2F2F7) and elevated interaction surfaces (#FFFFFF).

## Typography
This design system employs **Inter** for all primary interface text to ensure maximum legibility at various scales. A secondary typeface, **JetBrains Mono**, is used for telemetry data, coordinates, and status labels to evoke a technical, "instrument cluster" feel.

- **Headlines:** Use tight letter-spacing for a modern, compact look.
- **Body:** Standardized at 17px for the mobile-first PWA to ensure comfortable reading while in motion.
- **Labels:** Uppercase mono-spaced labels should be used for metadata and non-interactive status descriptions.

## Layout & Spacing
The layout follows a **Fluid Grid** model designed specifically for vertical mobile orientations. 

- **Touch Targets:** All interactive elements must maintain a minimum hit area of 48x48px.
- **Padding:** Use generous internal padding within cards (min 20px) to keep data points distinct.
- **Safe Areas:** The design system accounts for PWA "home screen" overlays, specifically maintaining a 34px bottom margin for gestures.
- **Vertical Rhythm:** Elements are stacked using an 8px base increment to maintain a consistent visual tempo.

## Elevation & Depth
Hierarchy is established through **Tonal Layers** combined with **Ambient Shadows**. 

- **Base Layer:** The background (#F2F2F7) acts as the canvas.
- **Interactive Layer:** White surfaces (#FFFFFF) sit atop the background with a very soft, diffused shadow (15% opacity Primary color, 12px blur, 4px Y-offset).
- **Active Overlay:** Modals and bottom sheets use a backdrop blur (10px) on the layers beneath them to maintain context while focusing user attention.
- **Pressed States:** Use a subtle inner-shadow or 2% darkening of the surface color to provide tactile feedback without excessive visual noise.

## Shapes
The shape language is friendly yet professional, utilizing significant rounding to make the interface feel modern and "human-centric."

- **Standard Elements:** Buttons and Input fields use the `rounded-lg` (16px) tokens.
- **Structural Containers:** Main dashboard cards and bottom sheets use the `rounded-xl` (24px) tokens to create a soft, protective frame around vehicle data.
- **Status Indicators:** Small indicators (like online dots) are always fully circular (pill-shaped).

## Components
Consistent styling across components ensures the vehicle remains easy to control under all conditions.

- **Primary Buttons:** High-contrast Navy or Tech Blue backgrounds with White text. Minimum height of 56px for critical actions.
- **E-STOP Button:** A specialized component. Large, centered, using the Danger Red (#FF3B30) with a subtle pulse animation when the vehicle is in a high-risk state.
- **Status Chips:** Small, semi-transparent backgrounds with high-contrast text (e.g., Light Green background with Dark Green text) to indicate vehicle "Health" or "Battery."
- **Data Cards:** White containers with a 1px stroke (#E5E5EA) and soft shadow. These house telemetry like speed, destination, and sensor feedback.
- **Progress Bars:** Smooth, rounded tracks with the Tech Blue fill for charging or distance remaining.
- **Input Fields:** Large, 16px rounded corners, using a light gray background (#E5E5EA) to differentiate from the primary white surface cards.