# Task Manager

A lightweight, privacy-first task manager that runs entirely in the browser — no installation, no account required.

---

## Overview

Task Manager is a single-file web application (`task_manager.html`) built with vanilla HTML, CSS, and JavaScript. All data is stored locally in the browser via `localStorage`. No data is ever transmitted to a server.

---

## Usage

### Via GitHub Pages (recommended)

Open the following URL in any browser:

```
https://pongpichetdinmuang.github.io/task-manager/task_manager.html
```

Bookmark it for quick access. Data persists in `localStorage` as long as the browser's site data is not cleared.

### Via local file

Download `task_manager.html` and open it directly in a browser. Note that `localStorage` is scoped to the origin, so data saved when running from `file://` is separate from data saved via GitHub Pages.

---

## Features

### Task Management
- Create, edit, and delete tasks
- Add a title, description, and deadline (date and time) per task
- Break tasks into subtasks; progress percentage is calculated automatically

### Urgency Classification

Urgency is derived automatically from the deadline. No manual input is required.

| Time Remaining | Level    |
|----------------|----------|
| < 48 hours     | Critical |
| < 72 hours     | High     |
| < 7 days       | Medium   |
| 7+ days        | Low      |
| Progress 100%  | Done     |

### Views
- **Overview** — summary stats (total, done, critical) and an aggregate progress bar across all tasks
- **Task detail** — full edit view with subtask management and countdown timer
- **Calendar** — monthly view with deadline dates highlighted; tap a date to navigate to that task

### Data Management

| Action | Behavior |
|--------|----------|
| Save | Writes current state to `localStorage` |
| Open file | Loads a previously exported `.json` file into memory; press Save to commit to `localStorage` |
| Export JSON | Downloads `tasks_data.json` to the device for backup or transfer to another browser/device |

---

## Data & Privacy

- All data is stored in `localStorage` on the user's device only
- No cookies, analytics, tracking, or external requests of any kind
- The exported `tasks_data.json` is a plain JSON file the user owns and controls

---

## Browser Support

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome  | Yes     | Yes    |
| Safari  | Yes     | Yes    |
| Edge    | Yes     | Yes    |
| Firefox | Yes     | Yes    |

---

## Tech Stack

- HTML / CSS / JavaScript (no frameworks, no build step)
- [Tabler Icons](https://tabler.io/icons) (loaded via CDN)

---

## File Structure

```
task-manager/
├── task_manager.html    # Application entry point
└── README.md
```

---

## License

MIT
