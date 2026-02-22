# Urban-Mobility-in-LATAM-Cities
Urban Mobility and Economic Productivity in LATAM Cities | Triple Ten 2026: To identify which cities to invest in transportation infrastructure in order to improve productivity and population well-being.
* **Objective:** To identify which cities to invest in transportation infrastructure in order to improve productivity and population well-being.
* **Data:** A unique, curated dataset was built from two different sources, applying data cleaning, standardization, and validation processes to heterogeneous variables.
* **Techniques:** Data manipulation and analysis using Python (Pandas, NumPy, Matplotlib, Seaborn), SQL queries, and descriptive statistics; process documentation in Jupyter Notebook with visualizations and an executive report.
* **Result:** It was demonstrated that there is no simple linear correlation between a city’s GDP per capita and its level of vehicular traffic, which made it possible to rethink investment criteria toward variables more relevant for public decision-making.

<div align="center">
  <img src="Urban Mobility/boxplot_jams_delay.png" alt="Boxplot jams-delay" width="60%" />
</div>
<br>

<div align="center">
  <img src="Urban Mobility/pib_per_capita.png" alt="PIB per cápita" width="60%" />
</div>
<br>

<div align="center">
  <img src="Urban Mobility/jams_economy.png" alt="Jams-Economy" width="60%" />
</div>
<br>

## Executive Summary

### **Context, Methodology, and Scope:**

- The analysis covered 15 major cities in Latin America during 2024, integrating mobility variables (TomTom) and economic variables (OECD). A rigorous data-cleaning process was applied, including standardizing column names to snake_case format (e.g., jams_delay, city_gdp_capita) and date conversion. For consolidation, daily data were aggregated into annual averages using .groupby, and both sources were merged with an INNER JOIN using city and year as keys, ensuring dimensional consistency of the dataset. Distributions were validated using histograms and boxplots, identifying an average delay of approximately 630 minutes and significant outliers.

### **Key Findings: Patterns and Anomalies:**

- Visual analysis shows that there is no simple linear correlation, but rather three distinct behaviors. First, the “Megacity Effect” (Mexico City and São Paulo), where high GDP per capita coexists with extreme congestion levels (jams_delay > 1700 min), suggesting that saturation is a byproduct of their economic dynamism. Second, the “Efficient Model,” represented by Montevideo, which has the highest GDP per capita in the group (approximately $26k) with minimal congestion (around 50 min), demonstrating that wealth does not necessarily imply traffic. Third, the “Low-Efficiency” group, where congestion is disproportionately high relative to the income generated.

### **Strategic Response: Priority City:**

- Addressing the central question, Bogotá is the city that shows the most critical relationship between high congestion and lower relative productivity. According to the data, Bogotá presents a very high accumulated delay (approximately 1,141 minutes, the third highest in the study) but a moderate-to-low GDP per capita (approximately $11,442), lower than Lima and far below that of other cities with similar traffic levels (Mexico City or São Paulo). This indicates a systemic infrastructure failure: the city loses productivity stuck in traffic without generating the compensatory wealth of large metropolises, making it the top candidate for urgent investment in mass transit.

### **Recommendations and Next Steps:**

- Prioritize Bogotá and Lima: Both cities require immediate mobility interventions (Metro/BRT) to unlock their economic potential.

- Data Validation (Santiago): An anomaly was detected in Santiago de Chile’s GDP data (approximately $2,277), which is suspiciously low given the country’s reality; it is recommended to audit the original source before making decisions about this city.

- Benchmarking with Montevideo: Study Montevideo’s urban planning policies to understand how it maintains high income levels with minimal vehicular friction.
