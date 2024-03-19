# Time Series Analysis and Intervention Detection

This Python project performs time series analysis and detects interventions in data, particularly focusing on changes over time and identifying significant drops as potential interventions. It's structured to process data from Excel files, analyze changes, segment data based on detected interventions, and forecast future values. This project is ideal for analyzing industrial, environmental, or any time-based data where interventions need to be identified, and future trends are of interest.

## Features

- **Data Preparation**: Loads data from an Excel file, filtering by specific criteria, and prepares it for analysis.
- **Intervention Detection**: Identifies significant drops in the data series as potential interventions.
- **Data Segmentation**: Segments the data based on identified interventions for detailed analysis.
- **Trend Analysis**: Calculates the slopes of different segments to understand trends.
- **Forecasting**: Predicts future values based on the identified trends and interventions.
- **Visualization**: Generates plots for each unique series, showing historical data, interventions, and forecasted values.

## Dependencies

- Python 3.x
- Pandas: For data manipulation and analysis.
- NumPy: For numerical operations.
- Matplotlib: For plotting and visualization.
- SciPy: For scientific computing, specifically linear regression here.

## Setup and Usage

### Initial Setup

Ensure you have Python 3.x installed along with the required libraries. You can install the dependencies using pip:

```bash
pip install pandas numpy matplotlib scipy
