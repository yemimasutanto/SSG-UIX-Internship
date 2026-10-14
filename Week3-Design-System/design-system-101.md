# Design System — Stready

A reusable set of colors, typography, spacing, and components built in Figma for the Stready marathon training companion. Every value below is a named style or variable in the Figma file, so screens reference the system instead of one-off values.

## 1. Color Palette

| Token | Name | Hex | Used for |
|-------|------|-----|----------|
| `Primary/600` | Deep Teal | `#0D7377` | Primary buttons (Apply, Save, Add Workout), active icons, active tab, selected states, progress fill |
| `Neutral/50` | Off-white | `#F5F7F7` | Screen background |
| `Neutral/0` | White | `#FFFFFF` | Cards, inputs |
| `Neutral/900` | Near-black | `#1A1A1A` | Headings, main body text |
| `Neutral/500` | Grey | `#6B7280` | Secondary text (labels, timestamps, helper text), inactive nav, input borders |
| `Neutral/200` | Light grey | `#E5E7EB` | Card borders, dividers, progress track |
| `Neutral/300` | Mid-light grey | `#D1D5DB` | Disabled elements, inactive chart bars |
| `Accent/400` | Amber | `#FBBF24` | Alerts and highlights (e.g. "Sick/Unwell" type reminders), used sparingly, always with dark text |

Usage balance: neutrals carry most of the interface, teal is the single action and selection color, and amber stays rare.

**Selected state rule:** anything selected or active (tab, date, chart bar, radio) uses `Primary/600`.

## 2. Typography

Font family: Inter

| Style | Size / Line height | Weight | Used for |
|-------|--------------------|--------|----------|
| Metric | 28 / 34 | Bold | Key numbers ("32.5 km", "65%") |
| H1 / Screen Title | 20 / 28 | Bold | Screen headers ("Training Calendar", "Workout Log") |
| H2 / Section Title | 16 / 22 | Bold | Section labels ("Quick Actions", "This Week") |
| Body | 14 / 20 | Regular | Card descriptions, instructions |
| Label | 12 / 16 | Medium | Timestamps, metadata (e.g. "6 km • 7:00/km • 42m") |
| Button text | 14 / 20 | SemiBold | Button labels |

Rules: every text element uses one of these named Text Styles, and the smallest text size is 12px.

## 3. Spacing & Layout

Spacing scale: 4, 8, 12, 16, 24, 32

| Token | Value | Used for |
|-------|-------|----------|
| Screen padding | 16px | Left/right margin on all screens |
| Card padding | 16px | Internal padding inside cards |
| Gap between cards | 12px | Vertical spacing between list items |
| Corner radius (cards) | 12px | Card corners |
| Corner radius (buttons) | 8px | Button corners |
| Icon circle size | 40px | Activity icon circles (Calendar/Log lists) |

## 4. Component Library

| Component | Variants / States | Notes |
|-----------|-------------------|-------|
| Button — Primary | Default, Pressed, Disabled | Teal fill, white text |
| Button — Secondary/Outline | Default, Pressed, Disabled | White fill, teal border, teal text (e.g. "View Details") |
| Card — Workout Item | Default, Pressed | Icon + title + metadata + chevron |
| Radio Button | Empty, Selected | Component variants (Week 2); unselected outline uses `Neutral/500` |
| Text Input | Default, Focused | Used for workout notes; border uses `Neutral/500` |
| Bottom Navigation | 4 states (Home / Calendar / Log / Profile active) | Icon + label; active = teal, inactive = `Neutral/500` |
| Progress Bar | — | Teal fill over `Neutral/200` track |
| Popup / Modal | — | White card, drop shadow, close (X) button |

## 5. Icons

- Icon set: Fluent Icons
- Activity icons: white icon on a solid teal circle (40px)
- Navigation icons: outline style, teal when active, grey (`Neutral/500`) when inactive

## 6. Accessibility Notes

Contrast ratios (WCAG AA requires 4.5:1 for normal text and 3:1 for UI components):

| Combination | Ratio | Result |
|-------------|-------|--------|
| White text on teal `#0D7377` | 5.62:1 | Pass |
| Teal text/icons on white | 5.62:1 | Pass |
| Teal text/icons on off-white `#F5F7F7` | 5.23:1 | Pass |
| Secondary grey `#6B7280` on white | 4.83:1 | Pass |
| Secondary grey `#6B7280` on off-white | 4.50:1 | Pass (at the limit) |
| Near-black `#1A1A1A` on amber | 10.43:1 | Pass |

Rules:
- Amber is used only as a fill or highlight with dark text, never as text or icon color on white (1.67:1).
- Secondary text is placed on white or off-white, never on a darker grey.
- Interactive component borders (inputs, unselected radios) use `Neutral/500`, not light greys.
- Minimum tappable area for buttons and icons: 44x44px.
- Icons are paired with text labels (bottom nav, quick actions), not icon-only.

## 7. Known Limitations (next iteration)

- Inactive chart bars (`#D1D5DB`) have low contrast against white (1.47:1). Values are also conveyed by bar height and day labels, and the selected day is highlighted in teal, but a stronger neutral should be tested.
- No error/destructive color is defined yet, because the current flows have no error state.
- Interaction states (pressed, disabled, focused) were defined for core components first; remaining components will be extended as the product grows.
