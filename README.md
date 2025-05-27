# 🌫️ Atmospheric CO₂ — Data Cleaning & Visualizations

This repository contains a cleaned, enriched version of the **Mauna Loa atmospheric CO₂ dataset** from NOAA and Scripps, along with a set of interactive **Tableau visualizations** that explore key trends in global atmospheric carbon dioxide concentrations.

---

## 🌍 Overview

The original dataset is sourced from the [Scripps Institution of Oceanography](https://scrippsco2.ucsd.edu/) and [NOAA Global Monitoring Laboratory](https://gml.noaa.gov/ccgg/trends/), which have maintained consistent CO₂ measurements at Mauna Loa Observatory since 1958. This repository focuses on:

- Cleaning and preparing the data for analysis  
- Creating interactive Tableau visualizations  
- Exploring long-term trends, seasonal cycles, and accelerating CO₂ growth

---

## 📁 Repository Structure

```plaintext
atmospheric-co2/
├── data/
│   ├── co2_monthly_raw.csv
│   └── co2_cleaned.csv
├── tableau/
│   └── co2_visualizations.twbx
├── notebooks/
│   └── co2_data_cleaning.ipynb
└── README.md
```

## ✨ Visualization Highlights

The Tableau visualizations include:

- 📈 **The Keeling Curve** – Atmospheric CO₂ trend from 1958 to present  
- 🔄 **Seasonal Fluctuations** – Annual CO₂ cycles and amplitude changes  
- 📊 **Rate of Change** – Year-over-year and decade-level growth comparisons  
- 🧭 **Annotated Trends** – Key moments such as international climate accords and volcanic events

---

## 🧹 Data Cleaning Summary

- Filtered invalid and flagged entries  
- Standardized column names and datetime formatting  
- Created derived features including:  
  - `yearly_increase`  
  - `5_year_rolling_avg`  
  - `anomaly_vs_baseline` (e.g., relative to 1960s mean)  
- Converted monthly records to datetime index for time series analysis

---

## 📊 Tools Used

- **Python (Pandas, Jupyter)** – For data processing and transformation  
- **Tableau Public** – For data storytelling and interactive visualizations

---

## 📦 Dataset Sources

- **Primary Source**: Mauna Loa Atmospheric CO₂ Monthly Averages  
- **Publishers**:  
  - [Scripps Institution of Oceanography](https://scrippsco2.ucsd.edu/)  
  - [NOAA Global Monitoring Lab](https://gml.noaa.gov/)  
- **License**: Public domain (see source-specific terms)  
- **Last updated**: May 2025

---

## 🚧 To Do

- [ ] Finalize and publish Tableau visualizations  
- [ ] Add comparative visualizations (e.g., emissions vs. CO₂)  
- [ ] Annotate policy milestones (e.g., Paris Agreement)  
- [ ] Conduct deeper feature engineering (e.g., rate of acceleration, seasonal shift detection)  
- [ ] Connect with other climate indicators for multi-variable insights

---

## 🙌 Acknowledgments

- Long-term atmospheric CO₂ records provided by **NOAA** and **Scripps**  
- Visualization inspired by tools like NASA’s [Vital Signs CO₂ Tracker](https://climate.nasa.gov/vital-signs/carbon-dioxide/)  
- Gratitude to climate scientists and data maintainers worldwide