# Daily-Energy-Demand-Forecasting-and-Optimization

This project involves forecasting daily energy demand and production, and optimizing energy supply strategies using various models. The project is divided into the following key components:

## 1. Data Preparation and Exploration

### Datasets
- **WeatherData.csv**: Contains weather-related data.
- **EnergyData.csv**: Contains energy demand and production data.

### Steps
1. **Load Data**: Imported the datasets and ensured data quality.
2. **Data Cleaning**: Removed duplicated columns and formatted date columns.
3. **Visualization**: Analyzed and visualized average energy demand and production by month.

## 2. Correlation Analysis

Merged weather and energy datasets to explore correlations between weather conditions and energy production. Created a heatmap to visualize the correlation between different features.

## 3. Forecasting Models

### Demand Forecasting
- **Model Used**: RandomForestRegressor
- **Features**: Average temperature and average wind speed
- **Performance**: Evaluated using RMSE

### Solar and Wind Forecasting
- **Model Used**: RandomForestRegressor
- **Correction**: Adjusted solar predictions where actual solar production was zero
- **Performance**: Evaluated using RMSE

## 4. SARIMAX Forecasting

### Model
- **SARIMAX Model**: Applied to forecast daily energy demand for the next 7 days.

### Results
Provided forecasts of daily energy demand for the upcoming week.

## 5. Optimization with Pulp

### Objective
Minimize energy supply costs while meeting average energy demand.

### Parameters
- **Grid Emission Factor**: 0.5
- **Solar Cost per kWh**: 0.05
- **Wind Cost per kWh**: 0.07
- **Natural Gas Cost per kWh**: 0.15

### Solution
Calculated optimal supply levels for grid, solar, and wind energy to meet demand at minimal cost.

## 6. Impact Assessment and Visualization

### Emissions Saved and Economic Savings
- **Emissions Saved**: Calculated the amount of CO2 emissions saved by optimizing the energy mix.
- **Economic Savings**: Compared the cost of energy supply with and without optimization.

### Results
- **Emissions Saved**: Displayed in kilograms of CO2.
- **Economic Savings**: Displayed in dollars.

### Visualizations
1. **Optimized Energy Supply Distribution**: Bar chart showing the distribution of energy supplied by grid, solar, and wind sources.
2. **Environmental and Economic Impacts**: Bar chart showing CO2 emissions saved and economic savings.

## Installation

Clone the repository:

```bash
git clone https://github.com/richardk100/ Daily Energy Demand Forecasting and Optimization.git
cd  Daily Energy Demand Forecasting and Optimization
