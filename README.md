# 📍 Mistake Tracker — A-Level Edition

A lightweight web app that helps A-Level students (Maths, Physics, Biology, Chemistry — Edexcel IAL) find out *exactly* where they're losing marks, instead of vaguely knowing they're "not great at Chemistry."

**Live app → [zarif-ops.github.io/alevel-mistake-tracke](https://zarif-ops.github.io/alevel-mistake-tracke/)**

<img width="1920" height="956" alt="image" src="https://github.com/user-attachments/assets/53726c4a-01d7-42b9-a813-f49ed170d70b" />


## Why I built this

While preparing for my own IAL exams, I kept making the same mistakes on past papers without realising it — losing marks in the same handful of subtopics again and again, but with no easy way to see the pattern. Spreadsheets were clunky and I didn't have anything that told me *what to actually revise next*. So I built the tool I wished I had, then generalised it so any A-Level student could use it.

## What it does

- **Log a mistake** in seconds after marking a past paper: subject → unit → topic → subtopic, marks lost, and *why* you lost them (conceptual gap, calculation error, misread question, time pressure, or a silly mistake)
- **Weighted weak-area ranking** — surfaces the subtopics actually costing you marks right now, weighting recent mistakes more heavily than old ones instead of just counting raw totals
- **Trend tracking** per subtopic — see whether a weak area is improving, stable, or getting worse over time
- **Error-type breakdown** — a chart showing whether you're mostly losing marks to careless mistakes vs genuine conceptual gaps, which calls for very different revision strategies
- **Local, private, and free** — all data stays in your own browser (no account, no server, no cost). Export/import to JSON if you want a backup.

## Why it's built the way it is

No backend, no database, no login — everything runs client-side and saves to the browser's local storage. That was a deliberate choice: it means the tool costs nothing to run or host, has zero setup for a new user (just open the link), and has no server-side privacy concerns since your data never leaves your device.

## Tech

Plain HTML, CSS, and JavaScript — no frameworks, no build step. Chart.js (via CDN) for the error-breakdown chart. Hosted free on GitHub Pages.

## Try it yourself

Just open the [live link](https://zarif-ops.github.io/alevel-mistake-tracke/) — no installation needed. Or clone this repo and open `index.html` directly in a browser.

## What I'd add next

- Cloud sync across devices (would need a lightweight backend)
- Per-subject predicted grade estimates based on logged performance
- Shareable weak-area reports for tutors/parents

---

Built solo by Zarif Hossain as part of independent A-Level exam preparation.
