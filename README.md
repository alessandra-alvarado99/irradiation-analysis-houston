# Solar Irradiation Analysis in Houston, Texas

### Objective: 
This project aims to estimate and compare the annual solar irradiation (kWh/m²) and average daily solar peak hours (HSP) across different zones of Houston, Texas. The purpose is to remotely evaluate the feasibility of photovoltaic system installations without requiring on-site inspections, thus improving initial client confidence.

## Parameters Used (via PVGIS API): 
- **Latitude and Longitude**: Used to represent key Houston area zones (e.g., Midtown, Galleria).
- **Peak Power**: Set to 1 kWp to normalize irradiation values.
- **Loss Factor**: 14% default system loss to approximate real-world PV losses.
- **E_y**: Total yearly energy product estimate (used to derive KWh/m²).

## Metrics Explained
- **Annual Irradiation (Kwh/m²)**: This indicates how much solar energy reaches a square meter of surface in a year. Higher values suggest better solar potential.
- **Daily HSP (Solar Peak Hours)**: Calculated by dividing annual irradiation by 365. Represents the equivalent number of full-sum hours per day (the average daily sunshine in Houston is around 5 hours).

## Tools
- **Python**: For data extraction and transformation.
- **PVGIS API**: Source of satellite-based solar data.
- **Power BI**: Used for creating geographic and comparative visualizations.

## Files
- **solar_irradiation_analysis.py** : Main script for collecting irradiation data.
- **solar_irradiation_houston_zones.csv**: Output CSV ready for visualization.

