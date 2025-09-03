# Low-Code Time Series & Geospatial Analysis of Madrid Air Quality

This repository contains a live MATLAB script that demonstrates **low-code workflows** for handling, analyzing, and visualizing **air quality** and **geospatial time series data** from several stations in Madrid, Spain.

## Project Overview

This project utilizes two datasets:

- [`madrid_2018.csv`](https://www.kaggle.com/datasets/decide-soluciones/air-quality-madrid): Hourly air pollutant measurements from various stations in Madrid.
- `stations.csv`: Geospatial information about each monitoring station (also from kaggle).

The script provides step-by-step methods to:
- Import and clean time series data.
- Handle missing values and outliers.
- Plot pollutant values across stations.
- Perform basic geospatial visualization.
- Explore signals with MATLAB’s built-in apps (e.g., `signalAnalyzer`).
- Use the curve fitting toolbox to compare polutants concentration 

## Requirements

- **MATLAB R2023b or later**
- Toolboxes:
  - Signal Processing Toolbox
  - Mapping Toolbox
  - Curve Fitting Toolbox
- Internet connection (to download datasets from Kaggle)

## Getting Started

1. **Download the data**  
   Visit [Kaggle Dataset Link](https://www.kaggle.com/datasets/decide-soluciones/air-quality-madrid) and download:
   - `madrid_2018.csv`
   - `stations.csv`

2. **Run the Live Script**  
   Open the `.mlx` version of this script in MATLAB.

3. **Explore Functionality**
   - Preview and clean datasets using the **Import Data App**.
   - Geospatially plot station data using `geoscatter`.
   - Smooth and analyze data using the **Signal Analyzer App**.
   - Generate comparison plots between pollutants (e.g., `NO` vs. `NO2`).

## Features Demonstrated

- **Data Import & Cleaning**  
  - Unstacking by station
  - Filling missing values
  - Handling outliers

- **Geospatial Visualization**  
  - Station map using latitude & longitude
  - Satellite basemap overlay
  - Station ID labeling

- **Time Series Analysis**  
  - Gaussian smoothing
  - Outlier detection with thresholds
  - Multi-panel plotting of station data

- **Signal Exploration**  
  - Launch `signalAnalyzer` for in-depth inspection

## Example Visualizations

> Plot NO data across all stations  
> ![Example plot placeholder](https://via.placeholder.com/400x200.png?text=NO+data+plot)

> Geospatial station map  
> ![Example map placeholder](https://via.placeholder.com/400x200.png?text=Station+Map)

## Author

**Kostas Leptokaropoulos**  
© 2025, The MathWorks, Inc.

