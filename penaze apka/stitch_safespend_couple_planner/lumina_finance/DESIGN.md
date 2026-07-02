---
name: Lumina Finance
colors:
  surface: '#111317'
  surface-dim: '#111317'
  surface-bright: '#37393e'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e8'
  on-surface-variant: '#c3c5d8'
  inverse-surface: '#e2e2e8'
  inverse-on-surface: '#2f3035'
  outline: '#8d90a2'
  outline-variant: '#434656'
  surface-tint: '#b7c4ff'
  primary: '#b7c4ff'
  on-primary: '#002681'
  primary-container: '#2d62ff'
  on-primary-container: '#f7f6ff'
  inverse-primary: '#004ceb'
  secondary: '#43ed9e'
  on-secondary: '#003920'
  secondary-container: '#00d084'
  on-secondary-container: '#005231'
  tertiary: '#ffb3ae'
  on-tertiary: '#68000b'
  tertiary-container: '#d62f34'
  on-tertiary-container: '#fff5f4'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b7c4ff'
  on-primary-fixed: '#001551'
  on-primary-fixed-variant: '#0039b5'
  secondary-fixed: '#59fead'
  secondary-fixed-dim: '#31e193'
  on-secondary-fixed: '#002111'
  on-secondary-fixed-variant: '#005231'
  tertiary-fixed: '#ffdad7'
  tertiary-fixed-dim: '#ffb3ae'
  on-tertiary-fixed: '#410004'
  on-tertiary-fixed-variant: '#930014'
  background: '#111317'
  on-background: '#e2e2e8'
  surface-variant: '#333539'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-numeric:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 40px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

The design system is engineered for a premium personal finance experience that balances institutional trust with modern agility. The brand personality is precise, transparent, and empowering, targeting a demographic that values data clarity and sophisticated aesthetics.

The visual style is **Corporate Modern with a Glassmorphic edge**. It utilizes a deep, multi-layered dark mode architecture to reduce eye strain during frequent financial check-ins. The interface relies on high-contrast data visualization and generous whitespace to ensure that complex financial information feels breathable and intuitive.

## Colors

The palette is anchored by a sophisticated "Ink" background (`#0F1115`), providing a deep canvas for high-chroma accents. 

- **Primary (Action):** A vibrant Electric Blue used for primary calls to action and global interactive states.
- **Success (Income):** A bright Emerald Green dedicated to positive cash flow, savings goals, and "Safe to Spend" indicators.
- **Error (Warning):** A crisp Vivid Red reserved for over-budget alerts, declined transactions, and critical warnings.
- **Info (Bills):** A Sky Blue used for recurring subscriptions and upcoming bill reminders.
- **Surface:** Secondary containers use a slightly lighter slate (`#1C1F26`) to create depth without sacrificing the dark aesthetic.

## Typography

This design system utilizes **Inter** for all primary communication to maintain a clean, neutral, and highly legible interface across all densities. To emphasize the precision of financial data, **JetBrains Mono** is introduced as a secondary font for transactional labels, account numbers, and currency tickers, providing a distinct "technical" feel to the numbers.

For mobile layouts, headline sizes scale down aggressively to ensure balance sheets and charts remain the focal point. Use `display-lg` exclusively for "Safe to Spend" balances and major total-wealth summaries.

## Layout & Spacing

The system follows a **Fluid Grid** model with an 8px base unit. 

- **Mobile:** A 4-column grid with 20px outside margins and 16px gutters.
- **Desktop:** A 12-column centered grid with a maximum content width of 1200px.
- **Safe Areas:** Maintain a 12px vertical buffer between the sticky bottom navigation and the scrollable content area.

Vertical spacing should favor a "tight" grouping of related data (8px) and "loose" separation between distinct financial sections (32px) to help users scan categories quickly.

## Elevation & Depth

Depth is achieved through a combination of **Tonal Layering** and **Ambient Shadows**. 

1. **Floor:** Background at `#0F1115`.
2. **Cards:** Surfaces at `#1C1F26`.
3. **Overlays:** Modals and menus use a backdrop blur (20px) with a 60% opacity fill of the surface color.

**Shadows:** Use extremely soft, long-range shadows for elevated cards. 
- *Style:* `0px 10px 30px rgba(0, 0, 0, 0.5)`. 
Avoid inner shadows or heavy borders. Interaction feedback should be shown through a subtle 1px border highlight (Primary Blue at 30% opacity) rather than a change in elevation.

## Shapes

The design system utilizes a **Rounded** (Level 2) language to evoke a friendly, modern feel that softens the "coldness" of financial data.

- **Standard Elements:** 8px (Buttons, small input fields).
- **Cards:** 16px (The primary container for all transaction lists and modules).
- **Featured Cards:** 24px (Large highlight cards like "Safe to Spend" or "Premium Upgrades").

Buttons and progress bar caps are fully pill-shaped (999px) to provide a clear distinction from information-bearing cards.

## Components

### Buttons
Primary buttons use the Primary Blue hex with white text, pill-shaped. Secondary buttons use a ghost style with a 1px border.

### Large 'Safe to Spend' Highlight Cards
The centerpiece of the dashboard. Use a subtle gradient (Primary Blue to Success Green) at 10% opacity for the background. The balance should be in `display-lg` typography. Ensure the card has a `rounded-xl` (24px) corner radius.

### Progress Bars
Track spending categories with a 8px height bar. The track should be the surface color (`#1C1F26`), while the indicator uses the category-specific accent color. Over-budget states should trigger a pulse animation on the indicator in Tertiary Red.

### Sticky Bottom Navigation
A fixed-position element with a heavy backdrop blur (Glassmorphism). Active states are indicated by the Primary Blue color and a small 4px dot below the icon.

### Cards & Lists
Transaction items should be grouped within a `rounded-lg` container. Use `body-sm` for timestamps and `label-numeric` for currency amounts. Positive amounts (Inflow) are always shown in Success Green.

### Input Fields
Inputs are borderless with a subtle `#1C1F26` background. Focus states are indicated by a 2px Primary Blue bottom-border only.