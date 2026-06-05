# Pool Inspector Calculator

**Camp Humphreys — Environmental Health Section**

Field calculator for aquatic facility inspections. Built on TB MED 575 and MAHC standards.

🔗 **[Open App](https://kimmybadger.github.io/Pool-Calc/)**

-----

## Calculators (11)

|# |Calculator                                    |Standard             |
|--|----------------------------------------------|---------------------|
|01|Pool Volume (Rectangular / Oval / L-Shape)    |—                    |
|02|Turnover Time                                 |TB MED 575 Table 2-2 |
|03|Required Minimum Flow Rate                    |TB MED 575 Table 2-2 |
|04|Pump Flow Rate (single or dual pump)          |TB MED 575 §2-35     |
|05|Bromine from TC reading (pool / spa / outdoor)|TB MED 575 §2-29     |
|06|Breakpoint Chlorination dose                  |TB MED 575 §2-26     |
|07|Langelier Saturation Index (LSI)              |TB MED 575 Appendix G|
|08|Spa Drain Interval                            |MAHC §5.7.3          |
|09|Spa Turnover Time (temp + bather density)     |MAHC Table 4.7.1.10  |
|10|Maximum Bather Load                           |TB MED 575 §2-16     |
|11|Pressure Converter (MPa / bar / kPa → psi)    |MAHC §4.7.2.2.5      |

-----

## Facility Data

Venue data is loaded from `facilities.json` in the repo root. Select facility and venue from the dropdown — volume and venue type auto-fill into calculators.

### Adding a new venue

Edit `facilities.json`:

```json
{
  "id": "gym_c_pool",
  "name": "Pool",
  "type": "pool",
  "location": "indoor",
  "volume_gal": 75000,
  "pump_count": 1,
  "note": ""
}
```

**Venue types:** `pool` · `spa` · `wading_pool` · `therapy_pool` · `catch_pool` · `activity_pool`  
**Locations:** `indoor` · `outdoor`

-----

## References

- **TB MED 575** (2015) — U.S. Army Recreational Waters Technical Bulletin
- **MAHC 4th Edition** (2023) — CDC Model Aquatic Health Code