# ⛅ Weather Dashboard

A **premium, Samsung-inspired weather dashboard** built with pure HTML, CSS & JavaScript. Search any city worldwide for real-time weather conditions, hourly forecasts, 5-day predictions, interactive weather maps, and moon phase data — all with a stunning animated UI.

---

## ✨ Features

| Feature                        | Description                                                                                            |
| ------------------------------ | ------------------------------------------------------------------------------------------------------ |
| 🌡️ **Real-Time Weather**       | Temperature, feels-like, humidity, wind, pressure, visibility                                          |
| 📅 **5-Day Forecast**          | Daily predictions with high/low temps and rain probability                                             |
| ⏰ **Hourly Forecast**         | Scrollable hourly breakdown with sunset marker                                                         |
| 📍 **Auto Geolocation**        | Detects your location on page load                                                                     |
| 🔄 **°C / °F Toggle**          | Instant unit switching across all temperatures                                                         |
| 🌅 **Sunrise & Sunset Arc**    | Animated SVG arc with glowing dot tracking the sun's real-time position                                |
| 🌔 **Moonrise & Moonset**      | Moon phase calculation with emoji, phase name, and approximate rise/set times                          |
| 🗺️ **Interactive Weather Map** | Leaflet.js map with satellite overlays — clouds, rain radar, temperature, wind                         |
| 🔍 **Smart City Search**       | Fullscreen overlay with auto-suggest (city + country flags) via Geocoding API                          |
| 🎨 **Dynamic Backgrounds**     | Gradient changes based on weather (blue for clear, grey for rain, etc.)                                |
| 🧑‍🎨 **Animated Characters**     | SVG human illustrations react to weather — umbrella for rain, beach vibes for sun, bundled up for snow |
| 💡 **Smart Tips Slider**       | Auto-cycling contextual tips (e.g. "Grab an Umbrella!")                                                |
| ☰ **Sidebar Menu**            | Saved cities ⭐, recent searches, popular cities, about section                                        |
| 💾 **Persistent Storage**      | Saved cities & recent searches stored in localStorage                                                  |

---

## 🖼️ UI Design

Inspired by the **Samsung Phone Weather App** & **Mausam App**:

- 💜 Soft purple/lavender gradient background
- 🪟 Translucent frosted card sections
- 📝 Inter font (Google Fonts)
- 🫧 Micro-animations: floating icons, swaying umbrella, falling snowflakes, drifting fog
- 🗺️ Interactive map with weather overlays & floating layer label
- 📱 Fully responsive — works on mobile & desktop

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- Internet connection (for API calls & fonts)

### Run Locally

```bash
# Clone the repository
git clone https://github.com/your-username/Weather_application.git

# Open in browser
cd Weather_application
open index.html    # macOS
start index.html   # Windows
```

> **No build tools needed!** Just open `index.html` directly in your browser.

---

## 📁 Project Structure

```
Weather_application/
├── index.html          # Main app — HTML structure + JavaScript logic
├── style.css           # Complete styling — Samsung-inspired design
├── images/
│   ├── clear.png       # Weather condition icons
│   ├── clouds.png
│   ├── drizzle.png
│   ├── humidity.png
│   ├── mist.png
│   ├── rain.png
│   ├── snow.png
│   └── wind.png
└── README.md
```

---

## 🔌 APIs

| Service                                                                      | Endpoint / Usage                                   | Purpose                            |
| ---------------------------------------------------------------------------- | -------------------------------------------------- | ---------------------------------- |
| [**OpenWeatherMap**](https://openweathermap.org/api)                         | `/data/2.5/weather`                                | Current weather data               |
| [**OpenWeatherMap**](https://openweathermap.org/api)                         | `/data/2.5/forecast`                               | 5-day / 3-hour forecast            |
| [**OpenWeatherMap Geocoding**](https://openweathermap.org/api/geocoding-api) | `/geo/1.0/direct`                                  | City auto-suggest search           |
| [**OpenWeatherMap Map Tiles**](https://openweathermap.org/api/weathermaps)   | `tile.openweathermap.org/map/{layer}/{z}/{x}/{y}`  | Cloud, temperature & wind overlays |
| [**RainViewer**](https://www.rainviewer.com/api.html)                        | `tilecache.rainviewer.com/{timestamp}/{z}/{x}/{y}` | Real-time rain radar imagery       |
| [**CartoDB**](https://carto.com/basemaps/)                                   | Voyager basemap tiles                              | Light map base layer               |

---

## 🗺️ Weather Map Layers

The interactive map card supports four switchable overlays:

| Toggle        | Source         | Data                            |
| ------------- | -------------- | ------------------------------- |
| ☁️ **Clouds** | OpenWeatherMap | Semi-transparent cloud cover    |
| 🌧️ **Rain**   | RainViewer     | Real-time precipitation radar   |
| 🌡️ **Temp**   | OpenWeatherMap | Color-coded temperature heatmap |
| 💨 **Wind**   | OpenWeatherMap | Wind speed visualization        |

---

## 🌙 Moon Phase System

Moon phase is calculated algorithmically using the **synodic month** (29.53 days) from a known new moon reference date. It displays:

- 🌑🌒🌓🌔🌕🌖🌗🌘 — Correct phase emoji
- Phase name (e.g. "Waning crescent")
- Approximate moonrise & moonset times

---

## 🌦️ Weather Character Guide

The animated SVG character in the hero section changes based on conditions:

| Weather     | Character                                                           |
| ----------- | ------------------------------------------------------------------- |
| ☀️ Clear    | Beach person — sunglasses, hat, Hawaiian shirt, flip flops          |
| ☁️ Cloudy   | Jacket person — scarf, hands in pockets                             |
| 🌧️ Rain     | Umbrella person — yellow raincoat, rain boots, animated drops       |
| ❄️ Snow     | Bundled person — beanie, puffer jacket, mittens, falling snowflakes |
| 🌫️ Mist/Fog | Scarf person — squinting eyes, long coat, drifting fog              |

---

## 🛠️ Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Grid, Flexbox, `backdrop-filter`, animations
- **JavaScript (ES6+)** — Async/await, Fetch API, Geolocation API, localStorage
- **SVG** — Inline animated character illustrations & sun arc
- **Leaflet.js** — Interactive map rendering
- **Google Fonts** — Inter typeface

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">
  Built with ❤️ | Powered by <a href="https://openweathermap.org/">OpenWeatherMap</a> · <a href="https://www.rainviewer.com/">RainViewer</a> · <a href="https://leafletjs.com/">Leaflet</a>
</p>
