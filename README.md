<div align="center">

# GeoTracker

**Real-time geolocation with interactive dark-themed map**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=leaflet&logoColor=white)

</div>

---

## About

GeoTracker is a modern geolocation web app that finds and displays your current position on a dark-themed interactive map. It uses the **browser Geolocation API** for high-accuracy GPS positioning, with automatic **IP-based fallback** when GPS access is denied or unavailable.

## Features

| Feature | Description |
|:--|:--|
| **GPS Positioning** | High-accuracy location via browser Geolocation API |
| **IP Fallback** | Dual API fallback (ipapi.co + ip-api.com) when GPS is denied |
| **Reverse Geocoding** | Displays approximate street address via Nominatim |
| **Dark Theme** | Full dark UI with CARTO dark map tiles |
| **Accuracy Circle** | Visual radius showing GPS precision |
| **Info Panel** | Animated panel with coordinates, accuracy, method, and address |
| **Custom Markers** | Styled blue marker with glow effect |
| **Responsive** | Works on mobile and desktop |

## How It Works

```
1. Page loads -> requests GPS permission
2a. GPS allowed -> shows high-accuracy position (zoom 16)
2b. GPS denied  -> falls back to IP geolocation (zoom 12)
3. Reverse geocoding resolves approximate address
4. Info panel slides up with all location data
```

## Tech Stack

- **Map Engine:** [Leaflet.js](https://leafletjs.com/) with CARTO dark tiles
- **Geolocation:** Browser Geolocation API (GPS)
- **IP Fallback:** [ipapi.co](https://ipapi.co/) + [ip-api.com](https://ip-api.com/)
- **Geocoding:** [Nominatim](https://nominatim.openstreetmap.org/) (OpenStreetMap)
- **Fonts:** [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts
- **No frameworks.** Pure HTML, CSS, and JavaScript.

## Usage

Just open `index.html` in any modern browser. No build step, no dependencies to install.

Or deploy to any static hosting (GitHub Pages, Vercel, Netlify).

## License

MIT
