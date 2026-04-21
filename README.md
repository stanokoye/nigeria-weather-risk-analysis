# Nigeria Weather Risk Analysis
### Seasonal Climate Intelligence for Event Planning — Abagana, Anambra State

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi&logoColor=white)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

## Overview

This is a personal research project initiated to support the planning of a significant family event — a chief's funeral in Abagana, Anambra State, Nigeria. What began as a practical question about weather became a structured data analysis exercise applying climate science, risk modelling, and data visualisation to a real-world decision.

The project demonstrates the full data analyst workflow: problem framing, data sourcing, cleaning, analysis, visualisation, and communication of findings to a non-technical audience.

> **Core question:** Which Thursday–Sunday weekend between mid-June and end of August 2026 carries the lowest rainfall risk for a three-day outdoor event in Abagana, Anambra State?

---

## Key Finding

**June 18–21, 2026 (Thu–Sun)** is the lowest-risk weekend in the research period.  
**Friday 19 June** carries the highest probability of a dry morning across all weekends studied.

Rain in late June is predominantly convective — short afternoon/evening thunderstorms — making it the most manageable pattern for scheduling outdoor ceremonial events.

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (pandas, matplotlib, seaborn) | Data cleaning, analysis, and chart generation |
| Power BI | Interactive dashboard and visualisation |
| Excel | Supporting data validation and cross-checking |
| Jupyter Notebook | Documented analysis workflow |
| GitHub | Version control and portfolio hosting |

---

## Project Structure

```
nigeria-weather-risk-analysis/
│
├── README.md                          # Project overview (you are here)
├── project_brief.md                   # Full methodology and problem framing
│
├── data/
│   ├── raw/                           # Original downloaded datasets
│   ├── processed/                     # Cleaned datasets ready for analysis
│   └── sources.md                     # Data sources and citations
│
├── notebooks/
│   └── 01_data_collection_cleaning.ipynb   # Data sourcing and cleaning
│
├── reports/
│   ├── Abagana_Weather_Report_2026.docx    # Full intelligence report
│   └── Abagana_One_Page_Summary.pdf        # Executive one-page brief
│
├── visuals/
│   └── powerbi/                       # Power BI dashboard files and exports
│
└── docs/
    └── methodology.md                 # Detailed methodology notes
```

---

## Data Sources

| Source | Type | Coverage |
|--------|------|----------|
| [WeatherSpark](https://weatherspark.com/y/52961/Average-Weather-in-Abagana-Nigeria-Year-Round) | Climate averages | 30-year historical averages for Abagana |
| [NiMet Seasonal Climate Predictions](https://nimet.gov.ng/scp) | Official forecast | 2020–2026 annual seasonal predictions |
| [NASA POWER](https://power.larc.nasa.gov/) | Satellite data | Daily climate parameters |
| [CHIRPS](https://www.chc.ucsb.edu/data/chirps) | Rainfall estimates | High-resolution precipitation data |
| Climates to Travel | Climate overview | Nigeria seasonal patterns |
| Springer (2010) | Peer-reviewed research | August break — eastern Nigeria |
| World Water Policy (2023) | Peer-reviewed research | Little Dry Season variability |

Full citations available in [`data/sources.md`](data/sources.md)

---

## Key Insights

1. **Late June has the most manageable rain pattern** — convective thunderstorms that are short, intense, and concentrated in the afternoon/evening (4–9pm), leaving mornings clear.

2. **The August break is unreliable in Anambra** — NiMet consistently rates southeastern Nigeria's Little Dry Season (LDS) as mild. Climate research confirms the break is weakening in the eastern humid zone due to climate change.

3. **August weekends carry the highest risk** — rainfall shifts to persistent, stratiform patterns that can last all day, with flood risk increasing significantly.

4. **Daily timing matters as much as date selection** — the 6am–1pm window is the safest across all weekends in the period.

---

## Deliverables

- [x] Full weather intelligence report (Word document)
- [x] One-page executive summary (PDF)
- [ ] Cleaned dataset (CSV)
- [ ] Jupyter Notebook — data collection and cleaning
- [ ] Power BI dashboard
- [ ] Methodology documentation

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/nigeria-weather-risk-analysis.git
cd nigeria-weather-risk-analysis

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook notebooks/01_data_collection_cleaning.ipynb
```

> Requirements file will be added as the notebook is built.

---

## About This Project

This project is part of my data analytics portfolio. It was driven by a real personal need — supporting the planning of a chief's funeral in Anambra State, Nigeria — and developed into a structured analysis exercise covering the full analyst workflow.

The goal is to demonstrate that data analysis skills apply to real, unstructured problems, not just classroom datasets.

**Skills demonstrated:**
- Research question framing and scoping
- Multi-source data collection and integration
- Data cleaning and preparation (Python/pandas)
- Exploratory data analysis
- Risk scoring and ranking methodology
- Data visualisation (matplotlib, Power BI)
- Communication of findings to non-technical stakeholders

---

## Author

**[Your Name]**  
MSc Business Analytics  
[LinkedIn](#) · [Portfolio](#)

---

*Data represents seasonal climate averages and probabilistic outlooks only. No long-range forecast can predict exact daily weather. Consult NiMet 7–10 days before any event for precise conditions.*
