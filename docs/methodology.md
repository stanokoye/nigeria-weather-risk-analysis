# Methodology — Nigeria Weather Risk Analysis

## Analytical Approach

This project uses a **seasonal climate outlook** approach rather than a point forecast. Weather beyond 10–14 days cannot be precisely predicted. Instead, the analysis relies on:

1. 30-year climatological averages to establish baseline expectations
2. NiMet Seasonal Climate Predictions to validate and contextualise year-to-year variation
3. Peer-reviewed climate research to assess the reliability of specific phenomena (the August break)
4. A relative risk index to rank weekends against each other

---

## Risk Index Construction

Each weekend was scored on a relative scale of 0–100 based on four factors:

### Factor 1 — Monthly rainfall probability (40% weight)
Based on average monthly rainfall (mm) and rainy days per month from 30-year data:
- June: ~200mm / ~18 rainy days
- July: ~200mm / ~20 rainy days
- August: ~199mm / ~20 rainy days

Late June weekends receive lower scores due to being earlier in the rainfall ramp-up.

### Factor 2 — Rain type and timing predictability (30% weight)
- **Convective (thunderstorms):** Driven by afternoon heat. Concentrated 4–9pm. Mornings clear. Lower disruption score.
- **Stratiform (persistent):** Widespread, all-day. No predictable window. Higher disruption score.

Late June = predominantly convective. August = predominantly stratiform.

### Factor 3 — August break adjustment (20% weight)
Weekends falling within the climatological August break window (approx. Jul 22 – Aug 5) receive a moderate downward adjustment — but this is capped due to the break's documented unreliability in southeastern Nigeria.

### Factor 4 — Flood risk (10% weight)
August weekends receive an upward risk adjustment reflecting the Anambra-Imo River Basin's documented susceptibility to flash flooding during peak August rainfall.

---

## Rain Type Classification

| Month | Dominant Type | Characteristics | Event Impact |
|-------|--------------|-----------------|-------------|
| Mid-June | Transitional | Mix of convective and early stratiform | Manageable |
| Late June | Convective | Short, intense, afternoon storms | Most manageable |
| Early July | Mixed | Increasing persistence | Moderate |
| Mid July | Stratiform | Prolonged, widespread | High |
| Late July | Stratiform / LDS | Possible lull (unreliable) | Moderate–High |
| August | Peak stratiform | All-day rain, flood risk | Very High |

---

## Daily Timing Model

Based on the convective rain pattern for the recommended June window:

| Time Window | Risk Level | Reasoning |
|-------------|-----------|-----------|
| 06:00–13:00 | Low | Pre-convective period. Solar heating insufficient to trigger storms. |
| 13:00–16:00 | Moderate | Heat building. Isolated showers possible. |
| 16:00–21:00 | High | Peak convective period. Storms most likely. |
| 21:00–06:00 | Low–Moderate | Storms dissipate. Overnight rain possible but less intense. |

---

## Limitations

See [`project_brief.md`](../project_brief.md) for full limitations statement.

Key limitations:
- No station-level observed data for Abagana
- August break behaviour is increasingly unpredictable due to climate change
- Risk index is relative, not absolute — it ranks weekends against each other within this period, not against all possible event windows globally

---

## Tools Used

| Stage | Tool | Output |
|-------|------|--------|
| Data collection | Python (requests, pandas) | Raw CSV files |
| Data cleaning | Python (pandas) | Processed CSV files |
| Exploratory analysis | Python (pandas, matplotlib) | Charts and summary tables |
| Risk modelling | Python (pandas) | Risk index scores |
| Visualisation | Power BI | Interactive dashboard |
| Reporting | Word, PDF | Intelligence report and one-pager |
| Version control | GitHub | Full project repository |

---

*Last updated: April 2026*
