---
name: Fortress Protocol
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
  on-surface-variant: '#44474d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#75777e'
  outline-variant: '#c5c6cd'
  surface-tint: '#515f78'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#0d1c32'
  on-primary-container: '#76849f'
  inverse-primary: '#b9c7e4'
  secondary: '#a04100'
  on-secondary: '#ffffff'
  secondary-container: '#fe6b00'
  on-secondary-container: '#572000'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#091b39'
  on-tertiary-container: '#7484a7'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d6e3ff'
  primary-fixed-dim: '#b9c7e4'
  on-primary-fixed: '#0d1c32'
  on-primary-fixed-variant: '#39475f'
  secondary-fixed: '#ffdbcc'
  secondary-fixed-dim: '#ffb693'
  on-secondary-fixed: '#351000'
  on-secondary-fixed-variant: '#7a3000'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#b6c6ed'
  on-tertiary-fixed: '#091b39'
  on-tertiary-fixed-variant: '#374767'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  h1:
    fontFamily: Public Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Public Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: Public Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Public Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Public Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  numeric-data:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is engineered to evoke an immediate sense of institutional security and financial authority. Targeting high-stakes users seeking credit recovery and constant monitoring, the personality is stoic, precise, and transparent. 

The visual style is **Corporate Modern** with a focus on data density and structural integrity. It utilizes a highly organized information hierarchy to reduce user anxiety during complex financial workflows. The aesthetic avoids unnecessary ornamentation, instead using clean borders and subtle depth to define "vault-like" containers for sensitive data.

## Colors

The palette is anchored by **Navy Blue (#0A192F)**, used to establish a "Deep Trust" foundation. This color is applied to headers, primary actions, and structural navigation to simulate a secure environment. 

**Alert Orange (#FF6B00)** serves as the high-visibility accent. It is reserved exclusively for critical status updates, credit score drops, and items requiring immediate user intervention. Backgrounds remain **White** or a very light **Slate Blue (#F8FAFC)** to ensure the interface feels clinical and uncluttered. Data visualizations utilize a secondary Navy (#112240) to create tonal separation without breaking the professional monochrome base.

## Typography

The typography strategy prioritizes legibility and an institutional feel. **Public Sans** is used for all core UI and headings due to its neutral, authoritative weight and clear character differentiation. For data-heavy contexts, **Inter** is employed to provide compact, functional labels and tabular numerals, ensuring credit scores and financial figures align perfectly in vertical lists.

Headings use tight letter-spacing and heavy weights to appear "locked-in" and stable. Body copy maintains a generous line height to prevent fatigue when reading legal disclosures or credit report details.

## Layout & Spacing

The design system utilizes a **Fixed Grid** model for desktop dashboards to maintain a controlled, dashboard-like environment where data density is predictable. On mobile, it transitions to a fluid single-column stack with 16px lateral margins.

A strict 8px base grid governs all spatial relationships. Components are spaced using a "Vertical Stack" logic—elements within a card use 12px or 24px gaps, while major page sections are separated by 48px to create clear cognitive breaks between monitoring tools and repair workflows.

## Elevation & Depth

Hierarchy is established through **Tonal Layers** and **Low-Contrast Outlines** rather than aggressive shadows. 

1.  **Base Layer:** White or #F8FAFC background.
2.  **Surface Layer:** White cards with a 1px border (#E2E8F0).
3.  **Elevated State:** Elements in focus or active "Action Cards" receive a subtle, ultra-diffused Navy-tinted shadow (Hex: #0A192F at 4% opacity, 12px blur, 4px Y-offset).

This approach ensures the UI feels "flat and sturdy" like a physical bank document, rather than floating or ephemeral.

## Shapes

The design system adopts a **Soft (0.25rem)** roundedness profile. This slight radius softens the professional aesthetic enough to feel modern and accessible without losing the structural discipline of a high-security product. 

Buttons and input fields use the standard 0.25rem radius. Secondary containers and "Security Gauges" may use circular (pill) shapes for progress indicators, but all primary structural elements (Cards, Modals, Forms) must strictly adhere to the soft-square geometry.

## Components

### Security-Focused Cards
Cards are the primary data vehicle. They must include a 1px solid border and a "Secure Header" area—often a 4px top-border in Navy or Orange to denote status. Information is segmented into internal rows with light horizontal dividers.

### Progress Gauges
Credit score visualizers should use semi-circular arcs. The stroke width must be substantial (12px+) with a flat cap. The gauge background is a light grey, with the active segment utilizing the Primary Navy or semantic success/error colors.

### Multi-Step Form Elements
To reduce friction in the "Repair" process, forms are broken into logical steps. Each step is displayed in a "Progress Track" at the top of the form. Active fields utilize a 2px Navy Blue border on focus, and inactive fields use a subtle grey background to indicate they are not yet reachable.

### Buttons & Inputs
*   **Primary Button:** Solid Navy Blue with white text; no gradient.
*   **Warning Action:** Alert Orange with white text for high-impact deletions or disputes.
*   **Input Fields:** Strictly rectangular with 4px radius; labels are always persistent (never placeholder-only) to maintain clarity.

### Security Badges
Small, high-contrast chips used to indicate "Verified," "Encrypted," or "Protected" status, often featuring a small padlock icon.