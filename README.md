# Road Accident Analysis Dashboard

> State-wise road accident analysis across India — cleaning multi-year data for 30+ states and building an interactive Power BI dashboard that identifies the highest-risk regions and fatality trends invisible in raw tables.

---

## Dashboard Preview

<img width="1238" height="700" alt="Dashboard Screenshot" src="https://github.com/user-attachments/assets/7e677d80-4cc3-4a34-8c9f-802cae1d2d3c" />


**Key Metrics at a Glance:**
- 18.98K average annual accidents across Indian states
- 4.50K average annual deaths
- 18.27K average injured per year
- 0.34 average fatality rate
- Maharashtra leads in total accidents (~85K) and deaths (~15K)
- Mizoram records the highest fatality rate (0.86) despite lower accident volume — a critical safety insight

---

## Problem Statement

Road accident data in India is reported state-wise across multiple years, making it difficult to spot which states are genuinely high-risk versus high-volume. This project answers:
- Which states have the highest accident and death counts?
- Which states have a disproportionately high fatality rate relative to accidents?
- Are fatality trends improving or worsening over time across regions?

---

## Dataset

- **Coverage:** 30+ Indian states and Union Territories, multi-year
- **Format:** Structured CSV (cleaned via Power Query ETL)
- **Key fields:** State/UT, Total Accidents, Total Deaths, Total Injured, Fatality Rate, Year

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Power Query | Data cleaning and ETL — zero manual row edits |
| Power BI | Interactive dashboard with map, bar charts, pie chart |
| Excel | Initial data inspection |

---

## Key Findings

- **Maharashtra** is the highest-risk state by volume — ~85K accidents and ~15K deaths
- **Mizoram** has the highest fatality rate (0.86) — meaning nearly 1 in 1 accident results in death, flagging a severe severity problem despite lower volumes
- **Top 5 high-risk states by accidents:** Maharashtra, Madhya Pradesh, Tamil Nadu, Karnataka, Rajasthan — these would be priority targets for any road safety policy brief
- Fatality rate distribution (pie chart) reveals that small states contribute disproportionately high rates, a finding completely hidden in raw accident count tables
- Cleaned multi-year data covering 30+ states using **Power Query ETL — zero manual row edits**

---

## Dashboard Features

- **KPIs:** Average accidents, deaths, injured, and fatality rate across all states
- **Map Visual:** State-wise accident distribution across India
- **Bar Charts:** Total accidents by state, total deaths by state (ranked)
- **Pie Chart:** Fatality rate distribution by state/UT
- **Slicer:** Filter by individual state for drill-down analysis

---

## Project Structure

```
road-accident-analysis/
│
├── data/
│   └── road_accidents_india.csv
│
├── dashboard/
│   └── road_accident_dashboard.pbix
│
└── README.md
```

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Prajjawal-kumar/Road-Accident-Analysis-Dashboard.git
   cd Road-Accident-Analysis-Dashboard
   ```

2. **Open Power BI Dashboard**
   - Open `dashboard/road_accident_dashboard.pbix` in Power BI Desktop
   - Data is embedded — no external connection needed
   - Use state slicers on the left to filter by region
