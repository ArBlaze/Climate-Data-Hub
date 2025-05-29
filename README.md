# 🌫️ Atmospheric CO₂ — Data Cleaning & Visualizations

This repository contains a cleaned, feature-rich version of the **Mauna Loa atmospheric CO₂ daily dataset** from NOAA and Scripps, paired with a suite of interactive **Tableau visualizations** that explore long-term trends, seasonal cycles, anomalies, and the accelerating pace of carbon dioxide accumulation in Earth's atmosphere.

---

## 🌍 Overview

The original dataset is sourced from the [NOAA Global Monitoring Laboratory](https://gml.noaa.gov/ccgg/trends/) and [Scripps Institution of Oceanography](https://scrippsco2.ucsd.edu/), which have maintained daily atmospheric CO₂ records at **Mauna Loa Observatory** since 1958. This repository focuses on:

- 🧹 Cleaning and enriching the raw daily CO₂ data using Python  
- 📈 Engineering temporal and statistical features for deeper insights  
- 🎨 Creating dynamic Tableau visualizations to tell the climate story

---

## 📁 Repository Structure

```plaintext
atmospheric-co2/
├── data/
│   ├── co2_daily_raw.txt
│   ├── co2_cleaned.csv
│   └── co2_with_features.csv
├── notebooks/
│   └── co2_cleaning_and_features.ipynb
├── tableau/
│   └── co2_visualizations.twbx
└── README.md
```

---

## ✨ Visualization Highlights

The Tableau dashboard includes:

- 📈 **The Keeling Curve** – Daily CO₂ concentrations from 1958 to present  
- 🔄 **Seasonal CO₂ Cycles** – Comparing yearly seasonal fluctuations (Earth’s “breathing”)  
- 🚀 **Rate of Increase** – Daily/monthly changes and rolling growth rates  
- 🌡️ **Anomaly Detection** – Outlier spikes and data irregularities highlighted  
- 📆 **CO₂ Heatmap** – Year vs. day-of-year heatmap for visual seasonal patterns  
- 🧭 **Polar Chart** – Radial view of seasonal CO₂ variation by day of year  
- 📊 **CO₂ Distribution Over Time** – Histogram and KDE of concentrations by decade  
- 🤖 **Forecasting (Optional)** – Predicted future CO₂ levels using statistical models

---

## 🧹 Data Cleaning & Feature Engineering

Data preparation in Python included:

- ✅ Filtered invalid entries (e.g., -99.99 values)
- ✅ Standardized datetime formatting
- ✅ Removed flagged records
- ✅ Filled missing values using interpolation or rolling averages

Engineered features include:

| Feature | Description |
|--------|-------------|
| `date`, `year`, `month`, `day`, `day_of_year` | Temporal decomposition |
| `co2_30d_avg`, `co2_365d_avg` | Rolling averages for trend smoothing |
| `daily_diff`, `monthly_diff`, `pct_change` | Rate of increase metrics |
| `anomaly_flag` | Detected outliers based on rolling mean/standard deviation |
| `sin_day`, `cos_day` | Cyclical encodings for seasonal/radial plots |
| `season` | Winter, Spring, Summer, Fall classification |
| `forecast` | Optional model-based future CO₂ estimates |

---

## 🛠️ Tools Used

- **Python (Pandas, NumPy, Matplotlib, Seaborn, Jupyter)** – For data cleaning and enrichment  
- **Tableau Public** – For dynamic, interactive data storytelling  
- *(Optional)* **Prophet / ARIMA** – For time series forecasting

---

## 📦 Dataset Sources

- **Primary Source**: Mauna Loa Daily CO₂ Concentration Data  
- **Publishers**:  
  - [NOAA Global Monitoring Lab](https://gml.noaa.gov/)  
  - [Scripps Institution of Oceanography](https://scrippsco2.ucsd.edu/)  
- **License**: Public domain (see publisher site)  
- **Last updated**: May 2025

---

## 🚧 To Do

- [ ] Finalize Tableau storytelling dashboards  
- [ ] Publish Keeling Curve animations using Pages Shelf  
- [ ] Add interactive filters for seasonality and anomalies  
- [ ] Explore comparative datasets (e.g., emissions, temperature rise)  
- [ ] Integrate CO₂ data with climate policy timelines

---

## 🙌 Acknowledgments

- Atmospheric CO₂ records courtesy of **NOAA** and **Scripps Institution of Oceanography**  
- Visual storytelling inspired by **NASA Vital Signs** and **Our World in Data**  
- Grateful to all scientists maintaining long-term climate datasets
