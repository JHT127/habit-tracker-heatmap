# Habit Tracker with Streak Heatmap

A simple, single-page habit tracker that helps you build consistency by visualizing your progress in a GitHub-style contribution heatmap.

## 🔗 Live Demo


## 📌 What It Does
- Add and remove daily habits you want to track
- Mark habits as done for the current day
- View your **current streak** and **longest streak**
- See your last ~90 days of activity in a color-coded heatmap, similar to GitHub's contribution graph
- All data is saved locally in your browser (no account or backend needed) via `localStorage`
- Toggle between light and dark mode

## 🛠️ Tech Stack
- **HTML** — page structure
- **CSS** — styling, layout (CSS Grid for the heatmap), dark mode via CSS variables
- **JavaScript (vanilla)** — all app logic, no frameworks or libraries
- **localStorage** — client-side data persistence

## ⚙️ How It Works
- Habits and daily completions are stored as JSON in `localStorage`
- The heatmap generates the last 90 days as date strings and maps each day's number of completed habits to a color intensity level
- Streaks are calculated by walking backward day by day from today, counting consecutive days with at least one completed habit
- All UI updates (habit list, streak count, heatmap) re-render automatically whenever data changes

## 🚀 Running It Locally
No build steps or dependencies required.
1. Clone this repo
2. Open `index.html` in your browser

## 💡 What I Learned
- DOM manipulation and event delegation
- Working with `localStorage` as simple client-side data storage
- Date manipulation in vanilla JavaScript
- Building a CSS Grid-based heatmap layout
- Implementing streak-calculation logic (a small but real algorithm)

## 📋 Project Info
Built as a Solo Project for the Chingu Developer Track (Tier 1).
