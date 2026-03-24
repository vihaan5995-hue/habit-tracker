# Habit Tracker

A personal habit tracking PWA built with vanilla HTML, CSS, and JavaScript. No frameworks, no backend, no dependencies. Works fully offline after the first load.

**Live:** `https://vihaan5995-hue.github.io/habit-tracker`

---

## Features

- Daily check-ins with a single tap
- Per-day notes alongside each habit
- Streak tracking and 7-day / 30-day completion rates
- Weekly heatmap view
- Browse and review any past date with notes intact
- Past dates are locked — habits cannot be retroactively modified
- CSV export and import for backup and device migration
- Rotating daily motivational quotes
- Dark mode, follows system preference automatically
- Fully offline via service worker (PWA)
- Installable on iOS, Android, and desktop

---

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire application |
| `sw.js` | Service worker for offline caching |
| `manifest.json` | PWA manifest for installability |

---

## Installation

### Add to iPhone (Safari)
1. Open the live link in Safari
2. Tap the **Share** button
3. Tap **Add to Home Screen**
4. Tap **Add**

### Add to Android (Chrome)
1. Open the live link in Chrome
2. Tap the **three-dot menu**
3. Tap **Add to Home Screen** or **Install App**

### Install on Desktop (Chrome / Edge)
1. Open the live link
2. Click the **install icon** in the address bar
3. Click **Install**

> Visit the link once on wifi. After that, the app works fully offline on all platforms.

---

## Data & Privacy

All data is stored in your browser's `localStorage`. Nothing is sent to any server — your habits are entirely private and stay on your device.

Things to be aware of:
- Data does not sync across devices or browsers
- Clearing browser data will erase your habits
- Use the Export feature regularly to keep a backup

---

## Backup & Restore

Open the **Progress** tab and scroll to the Backup section.

- **Export CSV** — Downloads a `.csv` file of your full habit history including notes
- **Import CSV** — Restores data from a previously exported file, merging with existing logs without overwriting

The exported file opens in Numbers (iOS), Excel, or Google Sheets.

---

## Daily Reminders (iOS Shortcut)

1. Open the **Shortcuts** app
2. Go to **Automation → New Automation**
3. Choose **Time of Day**, set your preferred time, repeat **Daily**
4. Add action: **Open URL** → paste your GitHub Pages link
5. Disable **Ask Before Running** → tap **Done**

---

## Deployment

Hosted via [GitHub Pages](https://pages.github.com/).

1. Upload `index.html`, `sw.js`, and `manifest.json` to a public GitHub repository
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Site goes live at `https://your-username.github.io/repo-name`

> When updating the app, bump the cache version in `sw.js` from `habit-tracker-v1` to `habit-tracker-v2` to ensure users receive the latest version.

---

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- `localStorage` for data persistence
- Service Worker for offline support
- GitHub Pages for hosting

---

## License

MIT — free to use, modify, and distribute.
