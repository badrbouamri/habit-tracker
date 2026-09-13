# Habit Tracker

An editable habit tracker: check off daily habits on a monthly grid, track weekly
habits, jot notes, and see an annual overview — all saved locally in your browser
(no backend, no account).

- `dist/index.html` — the live app. Plain HTML/CSS/JS, no dependencies, no build step.
  Data is stored in the browser's `localStorage`, so it's private to whatever device/
  browser you use the tracker from.
- `Habit Tracker.dc.html` — the original static design mockup this was visually based
  on, built with Claude Design's canvas editor (kept for reference; not deployed).
- `uploads/`, `_ds/` — design reference assets from that original mockup.

## Features

- Click a day cell to check a habit off; goals, progress bars and rings recompute live.
- Add, rename, or remove daily habits and their goals.
- Weekly habit checklists per week-of-month, editable per week.
- Editable notes (monthly and yearly).
- Month navigation — each month's data is kept separately.
- Annual overview aggregated from whatever months you've filled in.
- "Download Excel report" button exports the current month's habits, weekly checklist, and a
  year-long trend — including a computed improvement (percentage-point change) per habit — to
  an `.xlsx` file.

## Deploy

The `dist/` folder is a static site (no build step, no dependencies) and is deployed as-is to Vercel.
