# 🔌 Plugged — NYC Outlet Locator

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![Mapbox](https://img.shields.io/badge/Mapbox-GL-000000?logo=mapbox&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-Backend-6DB33F?logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)

Ever walked into a café desperately needing a charge, only to find zero available outlets? **Plugged** is a crowd-sourced web app that lets New Yorkers pin and share publicly accessible electrical outlets on an interactive NYC map.

Built as part of the [Tech Treks](https://engineering.nyu.edu/academics/programs/k12-stem-education/nyc-tech-talent-pipeline/tech-treks) program.

---

## Features

- 🗺️ **Interactive NYC map** — powered by Mapbox GL, constrained to NYC bounds
- 📍 **Add outlet locations** — search by address or click to drop a pin
- 🔍 **Address search** — Mapbox Geocoder for quick location lookup
- 📌 **Browse all pins** — view every crowd-sourced outlet location on load
- 🧭 **Geolocation** — find outlets near your current position

---

## Tech Stack

### Frontend *(this repo)*
| Technology | Purpose |
|---|---|
| React 18 | UI framework |
| react-map-gl 7 | Mapbox GL wrapper for React |
| @mapbox/mapbox-gl-geocoder | Address search |
| @turf/turf | Geospatial utilities |
| Webpack 5 | Bundler |

### Backend *(not in this repo)*
The backend was built with **Spring Boot** and a **MySQL** database, exposing a RESTful API for reading and writing outlet locations. It was developed locally and not committed to GitHub.

| Endpoint | Method | Description |
|---|---|---|
| `/api/show` | GET | Fetch all saved outlet locations |
| `/api/locations` | POST | Save a new outlet location |

---

## Getting Started

### Prerequisites
- A free [Mapbox token](https://account.mapbox.com/)
- Node.js 16+

### Installation

```bash
git clone https://github.com/ebc5802/outlet-map.git
cd outlet-map
npm install
```

### Environment Setup

```bash
cp .env.example .env
# Add your Mapbox token to .env
```

### Run

```bash
npm run start
```

### Build for production

```bash
npm run build
```

---

## Team

| Member | Role |
|---|---|
| Kevin Wang | Frontend |
| Andrew Lee | Frontend |
| Edison Chen | Backend |
| Chloe Han | Backend |
| Christopher Li | Backend |

📊 [View Presentation](https://drive.google.com/file/d/1-kG0LoLKk2ss7srXB0UOUbPYzE8v7KSu/view?usp=sharing)
