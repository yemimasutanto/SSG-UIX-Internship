# Information Architecture — Marathon Training Companion

## Site Map

```
Home (Dashboard)
├── Training Calendar
│   ├── Schedule Detail (per day)
│   ├── Add Record Workout (log results)
│   └── Suggest a Plan (Mode: "Suggest for me" — optional onboarding: level, target race, available days)
│
├── Workout Log
│   ├── Filter (All / Run / Walk / Other)
│   └── Workout Detail
│
├── Reschedule / Adjust
│   ├── Select Reason (Sick, Work, Weather, Tired, Other)
│   ├── Adjustment Suggestions (popup — multiple options + data behind each)
│   └── Reschedule Manually (fallback for coach-given / fixed plans)
│
└── Profile
    ├── Settings
    └── (Future) Connected Devices — smartwatch sync
```

## Navigation Structure

**Bottom navigation (persistent across app):**
`Home | Calendar | Log | Profile`

**Reschedule/Adjust** is accessed contextually — via a button/banner on Home and Schedule Detail — rather than living in the bottom nav, since it's an action triggered by a specific situation, not a destination users browse to regularly.

## Rationale (Design Decisions this reflects)

- **Two modes, one structure:** Both "I have my own plan" and "Suggest for me" modes share the same Training Calendar and Reschedule/Adjust flow — the difference is only in how the calendar gets populated (manual input vs. app-generated), keeping the IA simple rather than branching into two separate flows.
- **Reschedule Manually kept visible:** Based on Week 2 research, this option sits alongside auto-suggestions at the same level, not buried — since users with a coach-given plan need it just as often as the auto-suggestion path.
- **Workout Log separated from Calendar:** Calendar answers "what's planned," Log answers "what did I actually do" — keeping these separate avoids confusing planned vs. completed workouts in one view.
