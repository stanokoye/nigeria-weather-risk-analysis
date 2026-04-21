# Project Brief — Nigeria Weather Risk Analysis

## Problem Statement

A three-day outdoor event (a chief's funeral) is being planned in Abagana, Anambra State, Nigeria. The event spans Thursday to Sunday. The planning window under consideration is mid-June to end of August 2026. The question is:

> **Which weekend carries the lowest rainfall risk, and is the August break a reliable window to plan around?**

This is a real decision with real consequences — a state-level funeral with large community attendance, immovable ceremonial elements, and significant logistical investment.

---

## Scope

- **Location:** Abagana, Anambra State, Nigeria (6.18°N, 6.98°E)
- **Time period:** Mid-June to end of August 2026
- **Event format:** Thu–Sun (4-day window, 3 active event days)
- **Weekends assessed:** 10 consecutive Thu–Sun windows

---

## Methodology

### 1. Data Collection
- 30-year climate averages sourced from WeatherSpark for Abagana
- NiMet Seasonal Climate Predictions (SCP) reviewed for 2020–2026
- Peer-reviewed research on the Little Dry Season (LDS/August break) in southeastern Nigeria consulted
- Supplementary sources: Climates to Travel, Blue Green Atlas, Wikipedia Climate of Nigeria

### 2. Analysis Framework
- Monthly climate profile built for June, July, August (temperature, rainfall, rainy days, humidity, sunshine hours)
- Rain type characterised by month (convective vs. stratiform)
- Weekend-level risk index constructed based on:
  - Monthly rainfall probability
  - Rain type and timing predictability
  - Historical LDS behaviour for Anambra specifically
  - NiMet forecast patterns 2020–2025

### 3. Risk Scoring
Each weekend was assigned a relative risk index (0–100) based on:
- Expected rainy days in the 4-day window
- Rain type (convective = lower disruption, stratiform = higher)
- Monthly rainfall total and trend direction
- August break reliability for the southeast zone

### 4. Deliverables
- Full intelligence report (Word document, 8 pages)
- One-page executive summary (PDF)
- Cleaned dataset (in progress)
- Power BI interactive dashboard (in progress)
- Jupyter Notebook documenting full analysis (in progress)

---

## Key Variables

| Variable | Source | Notes |
|----------|--------|-------|
| Daily high temperature (°C) | WeatherSpark | 30-year average |
| Daily low temperature (°C) | WeatherSpark | 30-year average |
| Monthly rainfall (mm) | WeatherSpark | 30-year average |
| Rainy days per month | WeatherSpark | 30-year average |
| Humidity (%) | WeatherSpark / NiMet | Estimated range |
| Daily sunshine hours | WeatherSpark | 30-year average |
| LDS onset date | NiMet SCP | 2020–2025 predictions |
| LDS severity for Anambra | NiMet SCP | Mild in all available years |
| Rain type by month | Climate research | Convective vs. stratiform |

---

## Constraints and Limitations

1. **No station-level observed data** — Actual daily rainfall records for Abagana are held in NiMet's internal archives and are not publicly accessible. Analysis relies on climate averages and seasonal forecasts, not verified station observations.

2. **Seasonal averages ≠ exact forecasts** — 30-year averages describe what is typical, not what will happen. Exact conditions for any specific weekend in 2026 cannot be predicted at this range.

3. **August break uncertainty** — Peer-reviewed research confirms the LDS is weakening in southeastern Nigeria. NiMet rates Anambra's LDS as mild in all reviewed years. The break cannot be relied upon as a planning foundation.

4. **Climate change trend** — Published research projects increasing precipitation extremes in the Anambra-Imo River Basin in the near future, meaning historical averages may understate future rainfall intensity.

---

## Findings Summary

| Weekend | Risk Level | Recommendation |
|---------|-----------|----------------|
| Jun 18–21 | Moderate | **Best** — lowest risk in period |
| Jun 25–28 | Moderate–High | 2nd best |
| Jul 2–5 | High | Risky |
| Jul 9–12 | High | Risky |
| Jul 16–19 | High | Risky |
| Jul 23–26 | Moderate–High | August break window — not guaranteed |
| Jul 30–Aug 2 | Moderate | August break window — not guaranteed |
| Aug 6–9 | Very High | Avoid |
| Aug 13–16 | Very High | Avoid |
| Aug 20–23 | Very High | Avoid |

**Primary recommendation:** June 18–21, 2026  
**Most protected single day:** Friday 19 June (morning window, 6am–1pm)

---

## Next Steps

- [ ] Source and download NASA POWER daily data for Abagana coordinates
- [ ] Source CHIRPS rainfall estimates for the region
- [ ] Build and clean dataset in Python
- [ ] Construct risk model in pandas
- [ ] Build Power BI dashboard
- [ ] Document full workflow in Jupyter Notebook

---

*Brief prepared: April 2026 | MSc Business Analytics Portfolio Project*
