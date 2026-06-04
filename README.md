# Pool Inspector Calculator
**Camp Humphreys — Environmental Health Section**

A field reference calculator for aquatic facility inspections under TB MED 575 and MAHC (Model Aquatic Health Code).

---

## Features
14 calculators covering:
- Pool Volume (Rectangular / Oval / L-Shape)
- Turnover Time — with TB MED 575 pass/fail
- Required Minimum Flow Rate
- Dual Pump Flow (combined + single-pump fallback)
- Bromine from Total Chlorine reading
- Breakpoint Chlorination dose
- Cyanuric Acid compliance check
- Langelier Saturation Index (LSI)
- Spa Drain Interval (MAHC formula)
- Spa Turnover Time
- Maximum Bather Load
- Filter Pressure Drop
- Filter Flow Rate per Area
- Pressure Unit Converter (MPa / bar / kPa → psi)

---

## Usage
Open `index.html` in any browser. No installation or internet required for calculations.

Facility/venue data loads from `data/facilities.json`.

---

## Adding / Updating Facility Data
Edit `data/facilities.json` to add or update facilities and venues.

### Venue types
| type | Description |
|------|-------------|
| `pool` | Standard swimming pool |
| `spa` | Spa / hot tub |
| `wading_pool` | Wading / kiddie pool |
| `therapy_pool` | Therapy pool |

### Location values
- `indoor`
- `outdoor`

### Example entry
```json
{
  "id": "gym_c",
  "name": "Gym C",
  "venues": [
    {
      "id": "gym_c_pool",
      "name": "Pool",
      "type": "pool",
      "location": "indoor",
      "volume_gal": 75000,
      "pump_count": 2,
      "note": "Neptune-Benson dual filter system"
    }
  ]
}
```

---

## Hosting on GitHub Pages
1. Push this repo to GitHub
2. Go to Settings → Pages → Source: `main` branch / `root`
3. Access at `https://[username].github.io/[repo-name]`

---

## References
- **TB MED 575** (2015) — U.S. Army Recreational Waters Technical Bulletin
- **MAHC 4th Edition** (2023) — CDC Model Aquatic Health Code
