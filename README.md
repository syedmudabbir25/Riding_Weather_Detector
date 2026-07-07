# 🏍️ Riding Weather

A personal route-weather planning tool built for motorcycle and car riders in India. Plan your journey, pick your route, and know exactly where the weather turns bad — before you leave.

No app store. No sign-up. No API keys. One HTML file, works in any browser.

---

## What it does

Enter your starting point and destination, choose bike or car, set your departure time, and the tool calculates real road routes for you. Once you pick a route, it checks the weather forecast at checkpoints every 10–15 km along the road — not just at your destination — telling you the exact place and time where conditions might change. Rain, storms, fog, strong wind — you know before you ride.

---

## Features

### Route Planning
- Live place search with autocomplete — India-focused, cities shown before villages
- Paste coordinates directly — supports all three formats:
  - Plain decimal: `12.971599, 77.594566`
  - With direction: `12.971599N, 77.594566E`
  - DMS format: `12°58'17.8"N 77°35'40.4"E`
- Pin your start point, destination, or any stop directly on an interactive map
- GPS button to set your current location as the start point with one tap
- Add up to 8 stops along the route — the road is calculated through all of them
- Swap start and end with one tap
- Choose Bike or Car — routing and speed adjust automatically

### Route Selection
- Fastest route — minimum travel time, highway-focused
- Shortest route — minimum distance, fuel-saving
- Alternative route — shown when OSRM returns a genuinely different option
- If fastest and shortest are the same route (within 5 km and 10 min), shown as a single Best Route card
- All routes drawn on a live interactive map with colour coding
- Tap any route on the map or card to select it

### Weather Intelligence
- Checkpoints every 10 km (routes under 80 km) or 15 km (longer routes)
- Weather icons plotted on the map at each checkpoint so you see conditions visually across the whole route
- Four-level colour-coded severity at every checkpoint:
  - 🟢 Green — clear, safe to ride
  - 🟡 Yellow — light rain, mild wind, minor caution
  - 🟠 Orange — heavy rain, strong wind, high caution
  - 🔴 Red — storm, thunderstorm, dangerous
- Each checkpoint shows temperature, feels-like temperature, wind speed, and rain probability
- Live progress bar as checkpoints load — results appear in real time
- Ride verdict — Good to Go / Ride with Caution / High Caution / Avoid Riding
- Best time to ride — five windows across the day ranked by weather score
- Sunrise and sunset times for your travel date

### Saved Routes & Places
- Save any route (From + Stops + To + vehicle type) to a custom dropdown for instant reuse
- Each saved route has an inline delete button — no extra steps
- Heart button next to From and To fields saves individual places to favourites
- Saved favourites appear in a dedicated row below recent places with a green heart
- Recent places (last 4, deduplicated) shown as quick-tap chips
- All saved data persists in the browser — stays between sessions

### Sharing & Export
- Open in Google Maps — route with stops and vehicle mode pre-set, ready to navigate
- Share Link — copies or shares the Google Maps URL directly
- Copy Summary — full text summary including the Google Maps link, weather alerts, and all checkpoint details ready to paste into WhatsApp
- Notes clipboard — a small persistent scratchpad for coordinates, notes, or anything useful while planning

### Design
- Dark and light theme toggle, preference saved between visits
- Aston Martin racing green accent on a near-black chassis — minimal and intentional
- Phosphor Icons (thin weight) throughout — monochrome, Nothing OS inspired
- Rajdhani and JetBrains Mono typography for a technical, purposeful feel
- Fully mobile responsive — designed mobile-first since most rides are planned on a phone

---

## How to use

1. Open the file in any browser on desktop or phone
2. Select Bike or Car
3. Enter your departure point — type a city, paste coordinates, use GPS, or pin on the map
4. Optionally add stops
5. Enter your destination
6. Set date, start time, and average speed
7. Tap **Find Routes** and pick the route you want
8. Tap **Check Weather on Selected Route**
9. Review the verdict, best ride window, and checkpoint forecast
10. Share to Google Maps or copy the summary for your group

---

## Technology used

| Function | Service | Cost |
|---|---|---|
| Place search and autocomplete | OpenStreetMap Nominatim | Free |
| Route calculation | OSRM (Open Source Routing Machine) | Free |
| Weather forecast data | Open-Meteo | Free |
| Map display | Leaflet.js + OpenStreetMap tiles | Free |
| Route sharing | Google Maps URL scheme | Free |
| Icons | Phosphor Icons (thin weight) | Free |

**Total running cost — ₹0. No accounts, no API keys, no subscriptions required.**

---

## Installation

No installation needed. Download the `index.html` file and open it in Chrome, Firefox, or Safari. Works offline except for map tiles, routing, and weather data which need an internet connection.

To access it from your phone without transferring the file every time, host it free on GitHub Pages and open the link in your mobile browser. You can add it to your home screen from Chrome for an app-like experience.

---

## Notes

- Built as a single self-contained HTML file
- All saved routes, favourite places, and notes are stored in your browser's local storage — private to your device
- Designed for personal use in India — place search is India-focused by default
- Not affiliated with Google, OpenStreetMap, Open-Meteo, or OSRM
