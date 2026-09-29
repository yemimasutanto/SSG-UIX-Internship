# SSG-UIX-Internship
 
Documentation and deliverables for the **UI/UX Design Internship** at Skill Set Go EduTech (September–October 2026). This repo tracks the full 4-week journey — from research and wireframes to a finished, high-fidelity prototype and UX case study.
 
## About This Internship
 
A 4-week practical learning track covering UX fundamentals, user research, prototyping, usability testing, design systems, and a final UX case study capstone.
 
**Project:** Marathon Training Companion — unlike apps that "sell" a training program in place of a coach, this app's core role is to help runners track and stay accountable to a training plan they already have (self-made or coach-given), through reminders, progress tracking, and adaptive rescheduling when real life gets in the way. Suggesting a training menu is an optional, secondary feature — not the core value proposition.
 
## Repo Structure
 
```
├── Week1-Fundamentals/
│   ├── personas/
│   └── wireframes/
├── Week2-Research-Prototyping/
│   ├── journey-map/
│   └── prototype/
├── Week3-Design-System/
│   ├── components/
│   └── responsive-screens/
├── Week4-Case-Study/
│   ├── final-prototype/
│   └── case-study.pdf
└── certificates/
```
 
## Week-by-Week Progress
 
| Week | Focus | Status |
|------|-------|--------|
| Week 1 | UX principles, user personas, low-fi wireframes, high-fi Figma design | ✅ Done |
| Week 2 | User research, journey map, IA, interactive prototype, usability testing | ⬜ Not started |
| Week 3 | Design system, UI components, responsive design, accessibility | ⬜ Not started |
| Week 4 | Final product design, UX case study, presentation deck | ⬜ Not started |
 
## Problem & Target User
 
Runners preparing for a race often struggle to stick to a structured training plan when real life gets in the way — whether it's unexpected events, illness, work commitments, or lack of motivation. The target users are runners at two different stages: those preparing for their first race without a coach, and experienced runners balancing training with a demanding job.
 
## Research Summary
 
**Week 1 (persona research):** Lightweight research was conducted through self-reflection and short interviews with 2 experienced runners. Key finding: all respondents struggle with adjusting their training schedule when life disrupts it — either from unplanned events or work priorities. Experienced runners have also often tried multiple tracking tools (Garmin, Amazfit, Xiaomi, COROS) before settling on one they trust, showing that data accuracy and interface quality matter as much as features.
 
**Week 2 (feature validation):** Follow-up interviews with the same 2 runners validated the direction for the Reschedule/Adjust feature:
- Users don't want an app to act as the final authority on training decisions — an app can't account for variables like sleep or stress, so suggestions need to feel like options to weigh, not commands.
- Preference for being shown multiple options rather than one fixed suggestion.
- Neither respondent had prior experience with auto-suggestion features in a fitness context, meaning the UI needs to be self-explanatory rather than assume familiarity.
- Users want to see the data behind a suggestion (e.g. recent distance/intensity) before trusting it.
- Some runners follow a plan set by a personal coach and only need to input/track that program rather than have one generated for them — this shaped the app's positioning as a tracking/accountability tool first, with plan suggestion as an optional secondary feature.
See full persona documentation: `week-1-fundamentals/personas/`
 
## User Flow
 
The core UX direction, derived from persona research:
 
**Training Plan → Real-life disruption → Adaptive recommendation → Keep training on track**
 
## Design Decisions
 
The wireframes are structured around this direction. A dedicated **Reschedule/Adjust** flow was designed to suggest alternatives (not just skip a workout) when a session can't happen as planned — directly addressing the shared pain point found in both personas. Key screens include Home/Dashboard, Training Calendar, Workout Log, and Reschedule/Adjust, along with supporting detail and popup states.
 
Week 2 research reinforced this approach (multiple options over a single suggestion) and added two new design considerations:
1. **Transparency** — suggestions should surface the data behind them (e.g. recent distance/intensity), so users can evaluate rather than blindly follow.
2. **Two usage modes** — (a) *I have my own plan*, where users input/track a schedule they already have (self-made or coach-given), with the app focused on reminders, tracking, and reschedule-assist; and (b) *Suggest for me*, an optional mode for users who want the app to generate a training menu. The Reschedule/Adjust feature applies to both, though in Mode (a) it shifts an existing schedule rather than generating a new workout.
## Prototype
 
- Wireframes (Week 1): `week-1-fundamentals/wireframes/`
- Figma (high-fidelity): *[link]*
- Interactive prototype: *[link — coming in Week 2]*
## Usability Testing
 
*[Summary of usability test findings — coming in Week 2]*
 
## External Certificates
 
| Platform | Credential | Evidence |
|----------|------------|----------|
| Great Learning Academy | Figma for UI/UX Design | [Certificate PDF](https://github.com/yemimasutanto/SSG-UIX-Internship/blob/week-1-fundamentals/certificates/YemimaSutanto_GreatLearningAcademy_FigmaforUIUXDesign.pdf) |
| IBM SkillsBuild | | |
| Infosys Springboard | | |
| Simplilearn / HP LIFE | | |
 
## Next Improvements
 
*[What you'd refine further if you had more time]*
 
---
 
**Author:** Yemi
**Internship:** Skill Set Go EduTech — UI/UX Design Internship, Sep–Oct 2026
