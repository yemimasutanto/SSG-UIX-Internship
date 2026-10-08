# SSG-UIX-Internship

Documentation and deliverables for the **UI/UX Design Internship** at Skill Set Go EduTech (September–October 2026). This repo tracks the full 4-week journey — from research and wireframes to a finished, high-fidelity prototype and UX case study.

## About This Internship

A 4-week practical learning track covering UX fundamentals, user research, prototyping, usability testing, design systems, and a final UX case study capstone.

**Project:** Marathon Training Companion — unlike apps that "sell" a training program in place of a coach, this app's core role is to help runners track and stay accountable to a training plan they already have (self-made or coach-given), through reminders, progress tracking, and adaptive rescheduling when real life gets in the way. Suggesting a training menu is an optional, secondary feature — not the core value proposition.

## Repo Structure

```text
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

| Week   | Focus                                                                                          | Status        |
| ------ | ---------------------------------------------------------------------------------------------- | ------------- |
| Week 1 | UX principles, user personas, low-fi wireframes, high-fi Figma design                          | ✅ Done        |
| Week 2 | User research, journey map, information architecture, interactive prototype, usability testing | ✅ Done        |
| Week 3 | Design system, UI components, responsive design, accessibility                                 | ⬜ Not started |
| Week 4 | Final product design, UX case study, presentation deck                                         | ⬜ Not started |

## Problem & Target User

Runners preparing for a race often struggle to stick to a structured training plan when real life gets in the way — whether it's unexpected events, illness, work commitments, or lack of motivation.

The target users are runners at two different stages:

1. **Debut / self-training runners** preparing for their first race without a coach and needing structure, guidance, and accountability.
2. **Experienced runners** who already understand training but need flexibility when work, personal commitments, or other real-life circumstances interfere with their plan.

## Research Summary

### Week 1 — Persona Research

Lightweight research was conducted through self-reflection and short interviews with 2 experienced runners.

The main finding was that both respondents struggle with adjusting their training schedule when life disrupts it — either because of unplanned events or competing work priorities.

Experienced runners have also tried multiple tracking tools (including Garmin, Amazfit, Xiaomi, and COROS) before settling on one they trust. This highlighted that data accuracy and interface quality can be just as important as the number of features an app provides.

### Week 2 — Feature Validation

Follow-up interviews with the same 2 runners were used to validate the direction of the **Reschedule / Adjust** feature and refine the product concept.

Key findings:

* Users do not want an app to act as the final authority on training decisions. Factors such as sleep, stress, fatigue, and personal circumstances cannot always be understood by an app.
* Training recommendations should therefore be presented as **options to consider**, rather than commands.
* Users prefer seeing **multiple alternatives** instead of receiving one fixed recommendation.
* Neither respondent had prior experience with automatic training suggestions in a fitness context, meaning the feature needs to be self-explanatory.
* Users want to understand **why a recommendation is being made**, including relevant recent training data such as distance or workout intensity.
* Some runners already follow a training plan created by a personal coach. For these users, the primary need is to input, track, and stay accountable to an existing plan rather than generate a new one.

These findings reinforced the product positioning: **a training-plan tracking and accountability companion first, with training-plan suggestions as an optional feature.**

## User Flow

The core UX direction developed from the research is:

**Training Plan → Real-life disruption → Adaptive recommendation → Keep training on track**

The Reschedule / Adjust flow is designed to help users respond to missed or disrupted sessions without simply abandoning the training plan.

## Information Architecture

The prototype structure was organized around the user's core training workflow:

* **Home / Dashboard** — overview of current training progress and upcoming sessions
* **Training Calendar** — view and manage the overall training schedule
* **Workout Log** — review planned vs. completed workouts
* **Reschedule / Adjust** — respond to a disrupted workout and explore alternative options
* **Workout / Training Details** — inspect individual sessions and relevant training information

The architecture supports two potential usage modes:

1. **I Have My Own Plan** — users input or track an existing training schedule, whether self-made or provided by a coach.
2. **Suggest for Me** — users who want additional help can use the app's optional training-plan suggestion feature.

The Reschedule / Adjust feature can support both modes. In the first mode, it helps shift an existing schedule; in the second, it can help adapt a suggested plan.

## Design Decisions

Week 1 wireframes established the main screens and interaction structure. Week 2 focused on turning those structures into a more complete interactive prototype and validating the product direction through additional research and usability testing.

### 1. Recommendations as Options, Not Commands

The Reschedule / Adjust experience presents several possible alternatives instead of automatically deciding what the runner must do.

This reflects the research finding that runners want to retain control over their own training decisions.

### 2. Transparency Behind Recommendations

Recommendations should be accompanied by relevant training context, such as recent distance or workout intensity.

The goal is to help users understand the reasoning behind an option before deciding whether to follow it.

### 3. Existing Plan First

The app is positioned primarily as a **tracking and accountability tool** rather than another service that sells or replaces a coach-designed training plan.

Users who already have a plan should be able to bring that plan into the app and use the product to track progress, receive reminders, and adjust the schedule when necessary.

### 4. Interactive States

The Week 2 prototype introduced interactive UI states needed to make the core flows feel closer to a real product, including:

* Overlay menus and popup states
* Interactive selection controls
* Radio-button selection states
* Reschedule / Adjust interactions
* Prototype transitions between training-related screens

These interactions were added to move beyond static high-fidelity screens and demonstrate the intended user experience.

## Prototype

* Wireframes (Week 1): `Week1-Fundamentals/wireframes/`
* Journey map (Week 2): `Week2-Research-Prototyping/journey-map/`
* Prototype files (Week 2): `Week2-Research-Prototyping/prototype/`
* Figma (high-fidelity): *[link]*
* Interactive prototype: https://www.figma.com/proto/pFFZTPkFzBGS3rwcdSrmk9/Untitled?node-id=1-83&viewport=275%2C41%2C0.68&t=0rslMMcX9qeD3ZT4-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=1%3A83&page-id=0%3A1

## Usability Testing

A usability test was conducted to evaluate the core interactions of the prototype, focusing on three tasks:

1. **Rescheduling a training session** — finding the Reschedule / Adjust flow and understanding the available options.
2. **Logging a completed workout** — recording a 6 km run completed in 40 minutes.
3. **Checking weekly progress** — finding and understanding the user's weekly progress information.

The test was conducted remotely using screen recordings and post-task questions. The participant was asked to complete each task independently and rate the difficulty on a 1–5 scale.

### Task 1 — Rescheduling a Training Session

**Difficulty rating: 2/5**

The participant initially had difficulty finding the intended entry point and needed some time to become familiar with the prototype. However, after exploring the interface, they were able to reach the Reschedule page and understood the recommendation shown.

One issue was identified with the **"Reschedule Manually"** option. The participant attempted to interact with it, but the button was not accessible in the current prototype state, making it unclear that the option was available.

**Key finding:**
The Reschedule / Adjust entry point and interactive elements need stronger visual affordance so users can discover and interact with them more easily.

### Task 2 — Logging a Completed Workout

**Difficulty rating: 4/5**

The participant immediately navigated to the **Workout Log**, which matched the intended information architecture. However, they did not proceed to the **"Add Workout"** action because they assumed that reaching the Workout Log page was the end of the task.

As a result, they did not reach the workout input form where distance, duration, and pace could be entered.

**Key finding:**
The Workout Log page needs a clearer call-to-action for adding a new workout. The current design does not make the next step sufficiently obvious.

### Task 3 — Checking Weekly Progress

**Difficulty rating: 5/5**

The participant immediately identified the weekly progress information on the Home page and understood the displayed progress indicators, including **"65% Progress"** and **"Weekly Distance."**

The information was considered clear and easy to understand without additional guidance.

**Key finding:**
The current placement and presentation of weekly progress information effectively communicates the user's training status at a glance.

### Overall Feedback

The participant reported that the prototype was initially somewhat confusing because they were unfamiliar with the interface, but the experience became easier after exploring it.

The **Training Calendar** was the participant's favorite part of the application because it made it easy to view and manage the training schedule.

One additional feature request was the ability to manually add or display a **running route map** when recording a workout, so that the route could potentially be shared in a workout story.

### Usability Testing Limitations

The initial target was 2–3 usability testers. Four runners were contacted, but only **one participant completed the usability test** at this stage. One of the participants had also previously been interviewed during the app development process.

Therefore, the findings above should be treated as **initial usability insights rather than conclusive validation**. Additional testing with more runners would be needed to identify broader usability patterns and validate the proposed improvements.

## External Certificates

| Platform               | Credential             | Evidence                                                                                                                                                               |
| ---------------------- | ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Great Learning Academy | Figma for UI/UX Design | [Certificate PDF](https://github.com/yemimasutanto/SSG-UIX-Internship/blob/week-1-fundamentals/certificates/YemimaSutanto_GreatLearningAcademy_FigmaforUIUXDesign.pdf) |
| IBM SkillsBuild        |                        |                                                                                                                                                                        |
| Infosys Springboard    |                        |                                                                                                                                                                        |
| Simplilearn / HP LIFE  |                        |                                                                                                                                                                        |

## Next Improvements

The next stage will focus on strengthening the visual and interaction system rather than expanding the product scope.

Planned improvements include:

* Establishing a reusable design system and component library
* Standardizing typography, spacing, colors, and interaction states
* Improving responsive behavior across screen sizes
* Reviewing accessibility and interaction clarity
* Refining the prototype based on usability feedback
* Preparing the final product direction and UX case study

---

**Author:** Yemi
**Internship:** Skill Set Go EduTech — UI/UX Design Internship, Sep–Oct 2026
