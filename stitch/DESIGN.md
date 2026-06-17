---
name: PulseLog Mini
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
  secondary: '#515f74'
  on-secondary: '#ffffff'
  secondary-container: '#d5e3fd'
  on-secondary-container: '#57657b'
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
  secondary-fixed: '#d5e3fd'
  secondary-fixed-dim: '#b9c7e0'
  on-secondary-fixed: '#0d1c2f'
  on-secondary-fixed-variant: '#3a485c'
  tertiary-fixed: '#d3e4fe'
  tertiary-fixed-dim: '#b7c8e1'
  on-tertiary-fixed: '#0b1c30'
  on-tertiary-fixed-variant: '#38485d'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-metric:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  table-data:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '450'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  container-padding: 16px
  element-gap: 8px
  row-height-dense: 32px
  row-height-standard: 40px
---

## Brand & Style
The design system is engineered for operational efficiency, prioritizing deterministic interactions and high information density. The brand personality is reliable and calm, aimed at professionals who manage complex data streams within a compact interface. 

The aesthetic follows a **Modern Corporate** approach with a utilitarian focus. It avoids decorative elements in favor of functional clarity. The goal is to reduce cognitive load by using a structured layout that feels intentional and stable, ensuring that even under heavy data loads, the UI remains legible and unhurried.

## Colors
The palette is anchored in deep navy (`#0F172A`) for primary navigation and high-level structural elements, providing a sense of grounding and authority. 

- **Primary & Sidebar:** Use the deep navy for sidebar backgrounds and primary action buttons to establish a clear focal point.
- **Neutrals:** A range of slate grays is used for borders and secondary text. Backgrounds utilize very light cool grays (`#F8FAFC`) to maintain a clean, "app-like" feel without the starkness of pure white.
- **Semantic Colors:** Status indicators use standard but slightly desaturated tones to ensure they catch the eye without causing alarm. These should be used sparingly as small pips, thin borders, or subtle background tints.

## Typography
This design system utilizes **Inter** for its exceptional legibility at small sizes and its neutral, systematic character. 

- **Metrics:** For key operational data, use `display-metric` with a slight negative letter spacing to create a compact, "instrument panel" feel.
- **Data Grids:** The bulk of the interface uses `table-data` (13px). This size allows for high density while the 450 weight (Medium-Retina) ensures clarity on standard-resolution displays.
- **Labels:** Use `label-caps` for table headers and section titles to differentiate them clearly from the data they describe.

## Layout & Spacing
The layout follows a **fluid grid** with strict adherence to a 4px baseline. To achieve high density without clutter, the system uses "Purposeful Whitespace"—minimizing gaps between related items (8px) while maintaining clear 16px or 24px margins between major functional blocks.

- **Desktop:** 12-column grid, 16px gutter. Use a fixed-width sidebar (240px) and a fluid content area.
- **Information Density:** Tables and lists should default to a 32px row height for maximum data visibility. Use 16px horizontal padding within cells.
- **Reflow:** On smaller viewports, the sidebar collapses to an icon-only rail (64px) to preserve horizontal space for data tables.

## Elevation & Depth
Depth is communicated through **Tonal Layers** and **Low-contrast Outlines** rather than heavy shadows. This keeps the interface feeling "flat" and efficient.

- **Level 0 (Background):** Slate-50 (#F8FAFC) for the main canvas.
- **Level 1 (Cards/Sections):** Pure White (#FFFFFF) with a 1px solid border in Slate-200 (#E2E8F0).
- **Level 2 (Drawers/Popovers):** Pure White with a soft, 8px blur shadow (10% opacity, no spread) to indicate temporary overlay without detaching from the context.
- **Details Drawer:** Slides from the right, utilizing a full-height backdrop blur of 4px to maintain context of the underlying list.

## Shapes
The shape language is **Soft** and professional. A standard radius of 4px (`rounded-sm` or `0.25rem`) is applied to almost all elements including buttons, input fields, and cards. This provides a subtle modern touch while maintaining the structured, rectangular feel of a professional tool. Interactive components like checkboxes should retain this 4px radius, while circular elements are reserved exclusively for status pips and user avatars.

## Components
- **Buttons:**
  - *Primary:* Deep Navy background, white text. No gradient.
  - *Secondary:* Slate-100 background, Slate-900 text.
  - *Ghost:* No background, Slate-600 text; appears on hover with Slate-50 background.
- **Tables:** Headers are Slate-50 with 11px uppercase text. Rows use a 1px bottom border (#F1F5F9). Selected rows use a subtle blue tint (#EFF6FF).
- **Inputs:** 32px height for density. 1px Slate-300 border. On focus, the border changes to Primary Navy with a 2px soft blue glow.
- **Details Drawer:** A sliding panel for deep-dives into list items. It contains a header with the item title, a scrollable body for metadata, and a fixed footer for contextual actions.
- **Chips:** Small, 20px height tags with a 2px radius. Use light background tints of the status colors (e.g., Light Green background with Dark Green text for "Success").
- **Search:** A persistent input in the utility bar with a magnifying glass icon and a keyboard shortcut hint (e.g., "⌘K").