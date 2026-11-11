# Daymark — Daily Schedule Maker

A lightweight daily planner for college life. It runs as a static web page and saves your plans in the browser on the device you use.

## Features

- Daily timeline with date picker and previous/next-day navigation
- Add, edit, complete, and delete plans
- Start/end times, category, priority, notes, and reminder lead time
- Repeats: one date, every day, weekdays, or selected days
- Overlap warnings when plans collide
- Daily plan count, completion percentage, and upcoming items
- Browser notifications for reminders
- Export/import a JSON backup and export an `.ics` calendar file
- Responsive layout for desktop and mobile screens

## Run it

### Use GitHub Pages

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and `/(root)`, then save.
4. Open the Pages URL GitHub displays (usually `https://dumbummer.github.io/CollegeSched/`).

### Run locally

Open `index.html` in a modern browser. If notifications are unavailable from a local file, run a local static server, then open its localhost address:

```bash
python -m http.server 8000
```

## Reminders and data

Choose **Enable notifications** once and allow notifications in the browser. Set a reminder on each plan (at start, or 5–60 minutes before). Daymark checks reminders while the page is open. Keep the tab open for reminders; browser notifications cannot be scheduled after the page has been closed because this project has no server or push-notification service.

Plans are stored in that browser's local storage. They do not automatically sync between devices or browsers. Use **Export backup** and the import arrow to move your plan data. Use **Export calendar** to import events into another calendar app.

The planner does not include sample plans; add your own classes and routines using **＋ Add plan**.
