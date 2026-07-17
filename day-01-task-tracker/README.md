# Task Tracker

Part of the 100 Apps Challenge — Day 1

## Idea

A minimal, offline-first task tracker built as a single HTML file — no backend, no build step, just open it in a browser. Each task can be broken down into subtasks, with progress shown as a live percentage bar. It supports two people syncing their progress against each other (optional "Online Mode"), so you can hold yourself accountable alongside a friend without either of you having full visibility into — or control over — the other's list.

## How It Works

- **Local-first storage** — all tasks and subtasks are saved directly in the browser's `localStorage`. The app works fully offline with zero setup.
- **Tasks & subtasks** — create a task, break it into subtasks, and check them off. Progress percentage updates automatically per task and as an overall average.
- **Drag & drop reordering** — both tasks and subtasks can be reordered by dragging, independently of each other. Order is saved instantly.
- **Optional online sync** — connects to a simple Google Apps Script + Google Sheets backend (no server needed). When enabled, two users can see each other's full task lists, progress bars, and last-updated timestamps.
- **Fairness tracking** — if the gap between two synced users' average progress crosses a threshold, a warning appears so no one silently falls behind.
- **Auto-refresh timer** — online data refreshes automatically on a set interval (default: every 6 hours), with a visible countdown to the next sync, plus a manual refresh option.
- **Zero dependencies** — pure HTML/CSS/JavaScript in a single file.

## Stack

HTML, CSS, vanilla JavaScript, `localStorage`, Google Apps Script (optional backend for sync).
