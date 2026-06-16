# ⛰ Overland Ready — Camp Meal Planning

A mobile-first PWA for planning camp meals on overlanding trips. Part of the [Overland Ready](https://dbrinda.github.io/overland/) suite.

## Features

- **Meal planner** — day-by-day breakfast, lunch, dinner, snacks, and dessert across any number of trip days
- **Shopping list** — organized by category with progress tracking
- **Packing list** — cooler, dry storage, and gear categories with checkboxes
- **Swipe to delete** — swipe left on any item to remove it (scroll-safe)
- **⋮ Edit menu** — tap the three-dot icon to edit name, cook method tag, or delete
- **Undo / Redo** — persistent footer with full history (up to 50 steps)
- **Clear All** — wipes to a blank slate, fully undoable
- **Restore Defaults** — resets to the built-in 4-day solo trip plan
- **Cook method tags** — 🔥 Jetboil, ✓ No Cook, 🏕 Campfire, ❄️ Cooler
- **Offline support** — service worker caches the app on first load
- **PWA installable** — add to iPhone home screen via Share → Add to Home Screen
- **localStorage persistence** — data survives closing the browser

## Design

Matches the Overland Ready checklist app aesthetic:

- **Oswald** bold uppercase for headers and section titles
- **IBM Plex Mono** for body text and UI chrome
- Warm near-black background (`#0F0F0C`)
- Gold (`#C8A84A`) accent palette

## Deploy

Three files — drop them into any subdirectory of your GitHub Pages repo:

```
index.html      ← rename from camp-meal-planner.html
sw.js           ← service worker (offline caching)
manifest.json   ← PWA manifest (home screen install)
```

Recommended path: `dbrinda.github.io/camp-meals/`

Service worker activates on first load. After that the app works with no network connection.

## Default Trip

Pre-loaded with a 4-day solo overland meal plan:

|Day|Breakfast             |Lunch                   |Dinner          |
|---|----------------------|------------------------|----------------|
|1  |—                     |Deli wrap               |Tacos           |
|2  |Egg scramble burrito  |Deli wrap + cheese stick|Spaghetti       |
|3  |Egg scramble burrito  |Deli wrap               |Hot dogs + chili|
|4  |Oatmeal or protein bar|Deli wrap               |—               |

## Part of the Overland Ready Suite

- [Overland Ready Checklist](https://dbrinda.github.io/overland/) — full gear and pre-departure checklist
- [Utah Mighty Five Trip Guide](https://dbrinda.github.io/utah-mighty-five/) — 12-day PWA trip guide

-----

*Built for the GX 550 Overtrail+ and anyone who wants real food in the backcountry.*