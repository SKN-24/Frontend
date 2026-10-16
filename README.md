# Task Tracker

A clean, responsive Task Tracker built with **React + Vite** for the JTRONIX Frontend Internship Assessment. Tasks are stored in the browser's `localStorage`.


## Assessment checklist

### 1.1 Create and Display Tasks
- [x] Text box and **Add** button
- [x] Added tasks appear in a list
- [x] Empty (or whitespace-only) tasks are blocked, with an inline error and a shake animation

### 1.2 Manage Tasks
- [x] Mark each task **Completed** or **Pending** (checkbox and status badge)
- [x] **Delete** button on every task
- [x] Live counters for **Total**, **Completed** and **Pending**

### 1.3 Filter and Save Tasks
- [x] **All / Pending / Completed** filter
- [x] Tasks and statuses are saved in `localStorage` and survive a page refresh
- [x] Responsive layout for desktop and mobile

## Extra features

- **Progress ring** showing the completion percentage
- **Light / dark theme** toggle (remembers your choice, respects the system setting on first visit)
- **Priority levels** (High / Medium / Low) with colour coding, and smart sorting (pending first, then by priority)
- **Inline editing**: double-click a task or use the pencil button (Enter saves, Esc cancels)
- **Undo delete** toast
- **Search** box and **Clear completed** button
- **Confetti** when every task is completed
- **Keyboard shortcut**: press `/` to jump to the add box
- Time-aware greeting and motivational message
- Accessible: labelled controls, `aria-live` counters, visible focus states, reduced-motion support

## Run locally

Requirements: [Node.js](https://nodejs.org/) 18 or newer.

```bash
npm install
npm run dev        # starts http://localhost:5173
```

Production build:

```bash
npm run build      # outputs to dist/
npm run preview    # serves the built app locally
```

## Project structure

```
src/
  App.jsx             main component: state, filters, stats, task list
  Confetti.jsx        canvas confetti effect
  Icons.jsx           inline SVG icons
  useLocalStorage.js  custom hook that syncs state to localStorage
  styles.css          theme variables, layout and responsive rules
.github/workflows/deploy.yml   auto-deploy to GitHub Pages
```

