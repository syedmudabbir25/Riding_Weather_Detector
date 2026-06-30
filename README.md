# 🏍️ Riding Weather

A personal route-weather checker built for motorcycle and car riders in India. Plan your ride, pick your route, and see exactly where the weather might turn bad — before you leave home.

No app store, no sign-up, no API keys. Just open it in a browser.

---

## What it does

You enter where you're starting from, where you're headed, your vehicle type, and when you plan to leave. The tool calculates real road routes, breaks your journey into checkpoints every 10–15 km, and checks the weather forecast for the exact time you'll be at each one. If a storm, heavy rain, or strong wind is going to hit you somewhere along the way, you'll know the place and the time before you ever start the engine.

---

## Features

**Route planning**
- Search any place in India with live autocomplete suggestions
- Pin your start point, destination, or any stop directly on an interactive map — no typing needed
- Use your phone's GPS to set your current location as the starting point with one tap
- Add up to 8 stops along your journey; the route is calculated through all of them in order
- Choose between Bike or Car — routing and average speed adjust automatically
- See both the Fastest and Shortest route options side by side, drawn on the map, and pick the one you want

**Weather intelligence**
- Checkpoints every 10 km (short routes) or 15 km (longer routes) along your selected road
- Each checkpoint shows temperature, "feels like" temperature, wind speed, and rain probability
- Color-coded severity at a glance — green (clear), yellow (light caution), orange (heavy rain/wind), red (dangerous storm)
- Weather icons plotted directly on the map so you can see how conditions change visually across your route
- A live progress bar shows each checkpoint's weather loading in real time as it's fetched
- Overall ride verdict — Good to go / Ride with caution / High caution / Avoid riding
- "Best time to ride" — scans five time windows across the day and recommends the clearest one
- Sunrise and sunset times for your travel date, so you know if you'll be riding after dark

**Convenience**
- Save frequently used locations as favourites with one tap for instant reuse
- Light and dark theme toggle, remembered between visits
- Share your exact route — including all stops — directly to Google Maps with the correct vehicle mode (bike/car) pre-set for live navigation
- Copy a full text summary of your route and weather plan to paste into WhatsApp or share with riding group

---

## How it works (data sources)

| Function | Service used | Cost |
|---|---|---|
| Place search & autocomplete | OpenStreetMap Nominatim | Free |
| Route calculation (fastest/shortest) | OSRM (Open Source Routing Machine) | Free |
| Weather forecast data | Open-Meteo | Free |
| Map display | Leaflet.js + OpenStreetMap tiles | Free |
| Route sharing | Google Maps URL scheme | Free |

No accounts, no API keys, and no subscriptions are required for any part of this tool.

---

## How to use

1. Open the tool in any browser — desktop or mobile
2. Choose Bike or Car
3. Enter your starting point (type, use GPS, or pin on the map) and destination
4. Optionally add stops along the way
5. Set your travel date, start time, and average speed
6. Tap **Find Routes** and pick the route you want to take
7. Tap **Check Weather on Selected Route**
8. Review the verdict, best ride time, and checkpoint-by-checkpoint forecast
9. Share the route to Google Maps or copy the summary for your riding group

---

## Notes

- Built as a single self-contained HTML file — works offline except for the live map tiles and weather/routing API calls, which need an internet connection
- Designed mobile-first since most rides are planned and checked from a phone
- This is a personal-use tool and not affiliated with Google, OpenStreetMap, or Open-Meteo
