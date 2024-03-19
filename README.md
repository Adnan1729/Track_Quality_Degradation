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
```
## Running the Script

### Prepare your Excel file
Ensure your data is in an Excel file with at least two columns: one for dates and one for the values to analyze. The script expects columns named `MCAL_DAY_DT` for dates and `VAL_WT35` for values, along with a `STARTYARDAGE` column to filter the dataset for analysis.

### Modify the file paths
In the script, update the `file_path` and `output_dir` variables to point to your Excel file and the directory where you want the plots to be saved, respectively.

### Execute the Script
Run the script in a Python environment. The script will process the data for each unique `STARTYARDAGE` value, detect interventions, analyze trends, forecast future values, and generate plots for each series.

## Functionality Breakdown

- **Data Preparation**: Filters data based on `STARTYARDAGE` and prepares it for analysis by sorting and removing duplicates.
- **Detecting Interventions**: Looks for significant percentage drops in the series, marking these as potential interventions.
- **Segmenting Data**: Breaks the data into segments between interventions for separate analysis.
- **Trend Analysis and Forecasting**: Analyzes each segment to understand trends and uses this to forecast future values.
- **Visualization**: Generates a plot for each `STARTYARDAGE` series showing the historical data, marked interventions, and the forecasted future.

## Output

The script generates plots in the specified output directory, one for each unique `STARTYARDAGE` value in the dataset. These plots visualize the time series data, interventions, and forecasts, providing a comprehensive view of the data's behavior over time and potential future trends.
