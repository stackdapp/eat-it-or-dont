# Eat It or Don't 🍽️

Meal planning for people who hate meal planning.

## Features (v1)
- **Recipe Book** — add/edit/delete recipes manually or import from any URL
- **Meal Planner** — weekly calendar, assign recipes to any day/mealtime
- **Shopping List** — auto-generated from your meal plan + manual add
- **Print Mode** — print your planner or shopping list

## Tech Stack
- Vanilla HTML/CSS/JS
- Firebase (Auth + Firestore) — Google login, real-time sync across devices
- Claude API — recipe URL import

## Setup & Deploy

### 1. Firebase — Authorize GitHub Pages domain
1. Go to [Firebase Console](https://console.firebase.google.com) → your project
2. Authentication → Settings → Authorized domains
3. Add your GitHub Pages domain: `yourusername.github.io`

### 2. GitHub Pages
1. Create a new GitHub repo: `eat-it-or-dont`
2. Upload all files (index.html, style.css, app.js)
3. Go to repo Settings → Pages → Source: `main` branch, `/ (root)`
4. Your app will be live at `https://yourusername.github.io/eat-it-or-dont`

## File Structure
```
eat-it-or-dont/
├── index.html   ← entire app (Firebase + all logic)
├── style.css    ← all styles
├── app.js       ← placeholder for future expansion
└── README.md
```

## Notes
- All data stored in Firestore under each user's Google account
- Free Firebase tier is plenty for personal use
- No build tools required — pure static files
