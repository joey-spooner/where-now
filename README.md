# Where Now?

A simple, mobile-friendly web app for discovering food, outdoor, and cultural spots in the Lisbon area — Paço de Arcos, Cascais, Setúbal, and beyond.

## What it does

- Pick a category: **Food & Drink**, **Outdoor / Nature**, **Culture & Sites**, or **Wildcard**
- Set how much time you have (30 min → full day)
- Choose a starting point or use your GPS location
- Hit **Surprise me** to get a suggestion

The app factors in live weather from [Open-Meteo](https://open-meteo.com/) to bias towards indoor spots when it's raining and outdoor ones when it's sunny. It also tracks which places you've already seen today so you don't get repeats.

## Stack

Plain HTML, CSS, and vanilla JavaScript — no build step, no dependencies. Place data lives in `data/places.json`.

## Running locally

Just open `index.html` in a browser, or serve the folder with any static file server:

```bash
npx serve .
```

## Data

Places are stored in `data/places.json`. Each entry includes coordinates, category, indoor/outdoor classification, a TripAdvisor rating, notes, and a Google Maps link.
