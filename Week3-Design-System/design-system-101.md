# Design System — Marathon Training Companion

## 1. Color Palette

| Role | Color | Hex | Used for |
|------|-------|-----|----------|
| Primary | Deep Teal | `#0D7377` | Primary buttons (Apply, Save, Add Workout), active icons, active tab |
| Background | Off-white | `#F5F7F7` | Screen background |
| Surface | White | `#FFFFFF` | Cards, inputs |
| Text — Primary | Near-black | `#1A1A1A` | Headings, main body text |
| Text — Secondary | Grey | `#6B7280` | Labels, timestamps, helper text |
| Border/Divider | Light grey | `#E5E7EB` | Card borders, dividers |
| Alert/Warning | Amber | `#FBBF24` | Reminders, "Sick/Unwell" type alerts (used sparingly) |
| Neutral chart bars | Grey | `#D1D5DB` | Inactive bars in "This Week" chart |

> Fill in with your exact hex codes from Figma's color picker if any of the above differ slightly from what you applied.

## 2. Typography

| Style | Size | Weight | Used for |
|-------|------|--------|----------|
| H1 / Screen Title | 20px | Bold | Screen headers ("Training Calendar", "Workout Log") |
| H2 / Section Title | 16–18px | Bold | Section labels ("Quick Actions", "This Week") |
| Body | 14px | Regular | Card descriptions, instructions |
| Label | 12–13px | Medium | Timestamps, metadata (e.g. "6 km • 7:00/km • 42m") |
| Button text | 14–15px | Semibold | Button labels |

> Check your actual Figma text styles and replace these with your real values — if you haven't set named Text Styles yet, this is a good time to create them (select text → right panel → Text → create style icon) so they're reusable.

## 3. Spacing & Layout

| Token | Value | Used for |
|-------|-------|----------|
| Screen padding | 16px | Left/right margin on all screens |
| Card padding | 16px | Internal padding inside cards |
| Gap between cards | 12px | Vertical spacing between list items |
| Corner radius (cards) | 12px | Card corners |
| Corner radius (buttons) | 8px | Button corners |
| Icon circle size | 40px | Activity icon circles (Calendar/Log lists) |

> Adjust these to match what you've actually been using — open a few screens, select elements, and note the real values from the right panel.

## 4. Component Library

| Component | Variants | Notes |
|-----------|----------|-------|
| Button — Primary | Default, Pressed (optional) | Teal fill, white text |
| Button — Secondary/Outline | Default | White fill, teal border, teal text (e.g. "View Details") |
| Card — Workout Item | — | Icon + title + metadata + chevron |
| Radio Button | Empty, Selected | Built as component variants (Week 2) |
| Bottom Navigation | 4 states (Home/Calendar/Log/Profile active) | Icon + label, active = teal |
| Progress Bar | — | Teal fill over grey track |
| Popup/Modal | — | White card, drop shadow, close (X) button |

## 5. Icons

- Style: outline/filled consistent set (e.g. Fluent Icons, as already imported)
- Activity icons use a solid teal circle background with white icon
- Navigation icons use outline style, teal when active, grey when inactive

## 6. Accessibility Notes

- Text on teal background (`#0D7377`) uses white (`#FFFFFF`) for sufficient contrast
- Minimum tappable area for buttons/icons: 44x44px
- All icons are paired with text labels (bottom nav, quick actions) — not icon-only
