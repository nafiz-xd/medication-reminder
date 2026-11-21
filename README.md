# Medication Reminder

A calm, single-page medicine schedule manager that runs entirely in the browser. Add your medicines with their daily times, check off each dose as you take it, watch your stock count down with low-stock warnings, and see your weekly adherence at a glance. Everything is stored in your browser's localStorage — no account, no server, no data ever leaves your device. Reminders can fire as browser notifications while the app is open in a tab.

**Live demo: https://nafiz-xd.github.io/medication-reminder/**

## Features

- **Add, edit & delete medicines** — name, dose (e.g. "1 tablet"), total stock on hand, and an optional note.
- **Flexible schedules** — quick chips for Morning (08:00), Noon (13:00) and Night (22:00), plus as many custom times per day as you need.
- **Today view** — one card per scheduled dose across all medicines, sorted by time, with a big tap-to-check button; doses that are due and not yet taken get a gentle pulsing highlight.
- **Stock tracking** — checking a dose decrements stock by 1 (unchecking restores it), each medicine shows its stock and estimated days left, and a low-stock banner appears when any medicine has 3 or fewer days left. Checking is disabled when stock runs out.
- **Weekly adherence** — percentage of scheduled doses taken over the last 7 days, with a 7-bar mini chart showing each day's percentage. Medicines added mid-week are only counted from the day they were added.
- **Optional reminders** — enable browser notifications and get alerted when a dose time arrives (only while the app is open in a browser tab — there is no server).
- **Private by design** — all data lives in localStorage (`medrx_meds`, `medrx_checks`); nothing is sent anywhere.

## Tech

- Plain HTML, CSS and vanilla JavaScript — a single `index.html`, no build step, no dependencies.
- localStorage for persistence.
- Browser Notification API (feature-checked, best-effort) with a 30-second interval check.
- Soft mint/white medical theme with large, friendly tap targets and a responsive layout.

---

Built by Nafiz Bin Azad
