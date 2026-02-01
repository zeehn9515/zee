# Tashu JEE Dashboard (Offline)

## What this is
A lightweight offline web app for:
- Daily streak accountability
- Auto "today plan" based on Week 4→Final days roadmap
- Progress % (overall + week completion)
- PYQ shuffler from your uploaded PYQ bank (filtered for the target 80/20 topics)

## How to run (offline)
Option A (recommended): open a local server
1) Put this folder anywhere on your laptop.
2) In that folder, run:
   - Windows: `python -m http.server 8000`
3) Open: http://localhost:8000

Option B: open file directly
- Double-click `index.html`
(Works in most browsers because data is embedded.)

## How it saves data
- Stores progress in your browser's localStorage.
- Use **Stats → Export JSON** for backups and **Import JSON** to restore on another device.

## Notes
- PYQs show question text as extracted; answer keys are not included in the dataset.
- You can change streak rules (minimum PYQs per day) in Settings.


PWA/Offline: This build includes manifest.json + service-worker.js. After opening once online, it will work offline and can be installed on mobile ('Add to Home Screen').
