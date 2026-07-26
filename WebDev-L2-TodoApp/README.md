# WebDev-L2-TodoApp — Praneeth Madduri

**Track:** Web Development & Designing
**Task:** To-Do Web App

## Overview

An interactive to-do list app styled as a paper planner — ruled background, sticky-note style task cards, handwritten-style headers — with full add/complete/edit/delete functionality and persistence across page refreshes.

## Tech Stack

- HTML5
- CSS3 (Flexbox + Grid, custom properties for theming)
- JavaScript (Vanilla — no libraries or frameworks)
- Google Fonts: Caveat (handwritten headers), Inter (body), IBM Plex Mono (timestamps)

## Features

- Input field + "Add Task" button — new tasks appear instantly in Pending
- "Mark Complete" toggle moves a task between Pending and Completed lists
- Inline edit — click Edit to turn task text into an editable field (Enter to save, Escape to cancel)
- Delete permanently removes a task from either list
- Live count badges: "X pending" / "Y completed"
- **Bonus:** timestamps on every task (added date/time, and completed date/time once marked done)
- **Bonus:** tasks persist across page refreshes via `localStorage`
- Friendly empty-state messaging when a list has no items

## Architecture Note

A single `tasks` array (each with `id`, `text`, `completed`, `createdAt`, `completedAt`) is the one source of truth. The Pending and Completed columns are just filtered views of that array, re-rendered on every change — which keeps counts, persistence, and edit/delete logic from ever drifting out of sync.

## File Structure

```
WebDev-L2-TodoApp/
├── index.html      # Complete single-file app (HTML + inline CSS + JS)
├── README.md        # This file
└── screenshots/     # Add screenshots here before pushing
```

## How to Run

Open `index.html` directly in any modern browser — no build step or server required.

## Author

Praneeth Madduri — Information Science & Engineering Undergraduate, Malnad College of Engineering
praneethmadduri20006@gmail.com · github.com/praneethm · linkedin.com/in/praneethm
