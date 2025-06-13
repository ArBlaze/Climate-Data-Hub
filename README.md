# Clean Energy Displacement Timeline

## Project Overview

This project aims to visualize the pathway to net-zero emissions in the electricity sector by analyzing how much solar, wind, and hydroelectric power generation is required to displace fossil fuel-based electricity generation over time. Using historical data and future projections, the project will showcase the scale and pace of clean energy deployment needed to curb the effects of climate change by 2050.

---

## Data Sources

- **Our World in Data (OWID) Energy Dataset**  
  Provides historical electricity generation data by source (coal, gas, oil, solar, wind, hydro) from 1965 to present.  
  [https://github.com/owid/energy-data](https://github.com/owid/energy-data)

- **International Energy Agency (IEA) Net Zero by 2050 Roadmap**  
  Offers projections and targets for clean energy deployment required to achieve net-zero emissions by 2050.  
  [IEA Net Zero by 2050 Report (PDF)](https://iea.blob.core.windows.net/assets/deebef5d-0c34-4539-9d0c-10b13d840027/NetZeroby2050-ARoadmapfortheGlobalEnergySector_CORR.pdf)

---

## Methodology

1. **Data Preparation**  
   - Extract historical electricity generation data by energy source (coal, gas, oil, solar, wind, hydro) for the global scale (`country == "World"`).  
   - Calculate total fossil fuel electricity generation and total clean electricity generation (solar + wind + hydro).

2. **Projection Integration**  
   - Incorporate IEA’s net-zero scenario projections for clean energy deployment from 2023 to 2050.

3. **Displacement Calculation**  
   - Model the displacement of fossil fuel electricity by clean energy over time, maintaining electricity demand and accounting for relative efficiencies.

4. **Visualization**  
   - Use Tableau to create interactive timelines and charts comparing historical fossil fuel electricity with clean energy generation.  
   - Highlight progress toward net-zero and annual clean energy build-out requirements.

---

## Planned Visualizations

- **Electricity Generation Over Time:**  
  Line charts showing fossil fuel electricity vs. clean energy generation (solar, wind, hydro).

- **Displacement Percentage:**  
  Percentage of fossil electricity displaced by clean energy sources over time.

- **Scenario Comparison:**  
  Historical data vs. IEA projected clean energy deployment pathways.

---

## Getting Started

1. Download the latest OWID energy dataset CSV file.  
2. Filter and clean data as described in the methodology.  
3. Import the cleaned CSV into Tableau.  
4. Build visualizations based on the project goals.

---

## Tools and Technologies

- Data cleaning: Python (pandas) or Excel  
- Visualization: Tableau  
- Documentation and version control: Git/GitHub

---

## Contributing

Contributions and suggestions are welcome. Please open an issue or submit a pull request.

---

## License

This project is licensed under the MIT License.

---
