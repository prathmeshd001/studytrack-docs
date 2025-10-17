---
title: StudyTrack Pro — User Guide
---

# StudyTrack Pro — User Guide

**Version:** 0.1.0
**Last Updated:** 17 Oct 2025

StudyTrack Pro is a lightweight desktop/web tool to help students plan study sessions, track tasks, and generate simple progress reports.

---

## 1. Audience & Scope

This guide is for first‑time users (students) who want to create a study plan, track daily tasks, and generate a weekly report.

## 2. System Requirements

-   Windows 10/11, macOS 12+, or Ubuntu 22.04 and above
-   Node.js ≥ 18 (for the local web app)
-   Browser: Chrome, Firefox, Brave or Edge (latest)

## 3. Installation

### 3.1 Quick Start (Local Web)

```bash
# Clone the demo project
git clone https://example.com/studytrack-pro.git
cd studytrack-pro

# Install dependencies and run
npm install
npm run dev
```

Open the printed URL (usually `http://localhost:5173`).

### 3.2 Portable Desktop Build (Optional)

1. Run `npm run build`.
2. Package with your preferred bundler (e.g., Electron Forge).

## 4. First Run Wizard

On first launch, the wizard asks for:

1. **Semester length** (weeks)
2. **Courses** (names & credits)
3. **Target grade** (per course)
4. **Daily study window** (start/end time)

> Tip: Keep estimates realistic. You can edit everything later in **Settings → Planner**.

## 5. Key Concepts

-   **Plan** – A weekly template of study blocks.
-   **Task** – A to‑do item with due date, priority, and course tag.
-   **Session** – A timed focus block (e.g., Pomodoro 25/5).
-   **Report** – An auto‑generated snapshot of hours, completion, and slipage.

## 6. Creating Your First Plan

1. Go to **Planner → New Plan**.
2. Pick your weekdays and preferred time slots.
3. Drag a **Course block** onto the grid.
4. Click **Save as Default**.

**Common mistake:** Users sometimes forget to select a course before dragging. If you see a gray block with _No Course_, click it and set a course.

## 7. Adding Tasks

1. Open **Tasks → New**.
2. Enter a title (concise), choose a course, set **Priority** and **Due Date**.
3. (Optional) Add a checklist.
4. Click **Save**.

> Example: _Lab report draft_ with subtasks: outline → figures → references.

## 8. Starting a Focus Session

1. Go to **Focus** tab.
2. Choose a **Session type**: 25/5, 50/10, or Custom.
3. Click **Start**. Notifications will alert you when breaks occur.

> Note: Allow browser notifications to recieve (sic) break reminders.

## 9. Weekly Report

Navigate to **Reports → Weekly** and click **Generate**. The report includes:

-   Total hours per course
-   Tasks completed vs. planned
-   Top blockers and notes
-   Suggested adjustments

Click **Export** to save as PDF.

## 10. Settings

-   **Theme:** Light/Dark
-   **Backup:** Enable auto‑backup to local disk every 24h.
-   **Shortcuts:** Customize start/stop session hotkeys.

## 11. Troubleshooting

| Symptom               | Cause              | Fix                                                 |
| --------------------- | ------------------ | --------------------------------------------------- |
| Timer doesn’t start   | Browser tab asleep | Keep tab foreground or disable sleep in OS settings |
| Missing notifications | Browser blocked    | Allow notifications in Site Settings                |
| Report shows 0 hrs    | No sessions logged | Start a session or import from CSV                  |

## 12. FAQ

**Q:** Can I sync to phone?
**A:** Export your data and import on mobile web (planned native app coming soon).

**Q:** How do I collaborate?
**A:** Share exported plan JSON with peers, or co‑edit notes in Docs.

## 13. Privacy

All data stays on your machine unless you export or sync explicitly.

## 14. Glossary

-   **Slipage (sic)** – The difference between planned and actual hours. (should be _slippage_)
-   **Focus Ratio** – Minutes focused / total session minutes.

## 15. Changelog

-   **0.1.0 (2025‑10‑17):** Initial draft of user guide; known typos left intentionally for linting exercises (e.g., _recieve_, _slipage_).

---

## Appendix A — Sample Data

```json
{
    "courses": [
        { "name": "Algorithms", "credits": 4 },
        { "name": "Networks", "credits": 3 }
    ],
    "tasks": [
        {
            "title": "Lab report draft",
            "course": "Networks",
            "priority": "High",
            "due": "2025-10-25"
        }
    ]
}
```

# StudyTrack Pro — User Guide

**Version:** 0.1.0
**Last Updated:** 17 Oct 2025

StudyTrack Pro is a lightweight desktop/web tool to help students plan study sessions, track tasks, and generate simple progress reports.

---

## 1. Audience & Scope

This guide is for first‑time users (students) who want to create a study plan, track daily tasks, and generate a weekly report.

## 2. System Requirements

-   Windows 10/11, macOS 12+, or Ubuntu 22.04 and above
-   Node.js ≥ 18 (for the local web app)
-   Browser: Chrome, Firefox, or Edge (latest)

## 3. Installation

### 3.1 Quick Start (Local Web)

```bash
# Clone the demo project
git clone https://example.com/studytrack-pro.git
cd studytrack-pro

# Install dependencies and run
npm install
npm run dev
```

Open the printed URL (usually `http://localhost:5173`).

### 3.2 Portable Desktop Build (Optional)

1. Run `npm run build`.
2. Package with your preferred bundler (e.g., Electron Forge).

## 4. First Run Wizard

On first launch, the wizard asks for:

1. **Semester length** (weeks)
2. **Courses** (names & credits)
3. **Target grade** (per course)
4. **Daily study window** (start/end time)

> Tip: Keep estimates realistic. You can edit everything later in **Settings → Planner**.

## 5. Key Concepts

-   **Plan** – A weekly template of study blocks.
-   **Task** – A to‑do item with due date, priority, and course tag.
-   **Session** – A timed focus block (e.g., Pomodoro 25/5).
-   **Report** – An auto‑generated snapshot of hours, completion, and slipage.

## 6. Creating Your First Plan

1. Go to **Planner → New Plan**.
2. Pick your weekdays and preferred time slots.
3. Drag a **Course block** onto the grid.
4. Click **Save as Default**.

**Common mistake:** Users sometimes forget to select a course before dragging. If you see a gray block with _No Course_, click it and set a course.

## 7. Adding Tasks

1. Open **Tasks → New**.
2. Enter a title (concise), choose a course, set **Priority** and **Due Date**.
3. (Optional) Add a checklist.
4. Click **Save**.

> Example: _Lab report draft_ with subtasks: outline → figures → references.

## 8. Starting a Focus Session

1. Go to **Focus** tab.
2. Choose a **Session type**: 25/5, 50/10, or Custom.
3. Click **Start**. Notifications will alert you when breaks occur.

> Note: Allow browser notifications to recieve (sic) break reminders.

## 9. Weekly Report

Navigate to **Reports → Weekly** and click **Generate**. The report includes:

-   Total hours per course
-   Tasks completed vs. planned
-   Top blockers and notes
-   Suggested adjustments

Click **Export** to save as PDF.

## 10. Settings

-   **Theme:** Light/Dark
-   **Backup:** Enable auto‑backup to local disk every 24h.
-   **Shortcuts:** Customize start/stop session hotkeys.

## 11. Troubleshooting

| Symptom               | Cause              | Fix                                                 |
| --------------------- | ------------------ | --------------------------------------------------- |
| Timer doesn’t start   | Browser tab asleep | Keep tab foreground or disable sleep in OS settings |
| Missing notifications | Browser blocked    | Allow notifications in Site Settings                |
| Report shows 0 hrs    | No sessions logged | Start a session or import from CSV                  |

## 12. FAQ

**Q:** Can I sync to phone?
**A:** Export your data and import on mobile web (planned native app coming soon).

**Q:** How do I collaborate?
**A:** Share exported plan JSON with peers, or co‑edit notes in Docs.

## 13. Privacy

All data stays on your machine unless you export or sync explicitly.

## 14. Glossary

-   **Slipage (sic)** – The difference between planned and actual hours. (should be _slippage_)
-   **Focus Ratio** – Minutes focused / total session minutes.

## 15. Changelog

-   **0.1.0 (2025‑10‑17):** Initial draft of user guide; known typos left intentionally for linting exercises (e.g., _recieve_, _slipage_).

---

## Appendix A — Sample Data

```json
{
    "courses": [
        { "name": "Algorithms", "credits": 4 },
        { "name": "Networks", "credits": 3 }
    ],
    "tasks": [
        {
            "title": "Lab report draft",
            "course": "Networks",
            "priority": "High",
            "due": "2025-10-25"
        }
    ]
}
```
