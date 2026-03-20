# horse-blanket

Web app for Efona Ranch that tells horse owners whether their horse needs a blanket tonight. Uses overnight minimum temperature and coat type to give a yes/no recommendation.

## Features

- **Veterinary blanket thresholds** — temperature cutoffs based on coat insulation (clipped: below 15°C, short: 10°C, long: 5°C, winter: 0°C)
- **4-level coat type slider** — clipped, short, long, winter
- **Multi-model averaging** — combines Best Match, GFS, and ECMWF forecasts for more reliable overnight minimums
- **Feels-like temperature** — uses apparent temperature (wind + humidity) for blanket decisions
- **7-day overnight forecast** — overnight lows for each night with blanket recommendation
- **Mobile-friendly layout** — responsive, RTL Hebrew

## Quick Start

```bash
cd horse-blanket
python3 server.py
```

Open http://localhost:9999

## Usage

1. Open the page — forecast loads from Open-Meteo (location: Efona Ranch)
2. Select coat type via the slider
3. View tonight's recommendation and the 7-day overnight forecast
