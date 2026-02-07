*Rainfall in Dublin & Cork (Before vs After 2020)*

This project analyses long-term rainfall patterns in Ireland by comparing daily rainfall totals at Dublin Airport and Cork Airport, split into two periods: Before 2020 and After 2020.
Hourly meteorological data from Met Éireann is cleaned, aggregated to daily values, and visualised using a single interactive violin plot to highlight distributional differences, variability, and extreme rainfall events.

*Dataset:*
Source: Met Éireann – Historical Climate Data
https://www.met.ie/climate/available-data/historical-data

1.Stations
  Dublin Airport (1945–2025)
  Cork Airport (1962–2025)
  
2.Raw data:
  Hourly observations
  ~1.9 million rows combined

3.Variables used:
  Rainfall (mm)
  Air temperature (°C)
  Relative humidity (%)
  Timestamp (UTC)

4.After cleaning and aggregation:
  Dublin daily rows: 29,525
  Cork daily rows: 23,316
  Total daily records: 52,841

*Data Processing:*
Steps performed in Python:
Removed metadata rows from raw CSV files
Parsed timestamps into datetime format
Converted rainfall values to numeric
Removed invalid or negative values
Aggregated hourly data into daily totals

*Visualisation:*
The final output is one interactive violin plot comparing:
Dublin — Before 2020
Dublin — After 2020
Cork — Before 2020
Cork — After 2020

*What the plot shows?*

Violin shape → rainfall distribution (density)
Inner box → quartiles
Points → outliers (extreme rainfall days)
Black dot + label → mean daily rainfall
This satisfies the requirement for one sophisticated explanatory visualisation.

*Key Findings:*
Cork consistently receives more rainfall than Dublin.
Cork shows higher variability and more extreme rainfall events.
Both stations show a slight increase in mean rainfall after 2020.
The increase is more pronounced in Cork than in Dublin.

*Files in This Repository:*
RainDVM.ipynb – Full data processing and visualisation notebook
RainDVM.docx / Data_Visualisation_Assignment_Pair.pdf – Project report
dublin_daily_rain.csv – Cleaned daily rainfall (Dublin)
cork_daily_rain.csv – Cleaned daily rainfall (Cork)
final_interactive_violin.html – Interactive Plotly visualisation

How to Run:
copy paste this "pip install pandas plotly"

Open(text) and run:
RainDVM.ipynb

*Tools Used:*
1.Python
2.pandas
3.Plotly
4.Jupyter Notebook
