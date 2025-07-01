# FCC Forum Page View Visualizer

This project analyzes and visualizes page view data from the freeCodeCamp.org forum. It uses Python with pandas, matplotlib, and seaborn to generate various plots, providing insights into daily page views, monthly averages, and yearly/monthly distributions.

## Project Overview

The primary goal of this project is to:
1. Load and clean forum page view data from a CSV file.
2. Visualize daily page views over a specified period.
3. Show average daily page views for each month, grouped by year.
4. Display the distribution of page views by year and month using box plots.

The analysis helps in understanding trends and seasonality in forum traffic.

## Features

- **Data Cleaning:** Filters out days with page views in the top 2.5% or bottom 2.5% of the dataset to remove outliers.
- **Line Plot:** Shows daily page views from May 2016 to December 2019.
- **Bar Plot:** Displays average monthly page views grouped by year.
- **Box Plots:** Two adjacent box plots showing:
    - Year-wise distribution of page views (Trend).
    - Month-wise distribution of page views (Seasonality).

## Files Generated

The script `fcc.ipynb` (when run as a Python script or notebook) will generate the following image files:
- `line_plot.png`: Daily page views over time.
- `bar_plot.png`: Average monthly page views by year.
- `box_plot.png`: Distribution analysis by year and month.

## Requirements

The project relies on the following Python libraries:
- pandas
- matplotlib
- seaborn
- numpy

These dependencies are typically included in standard Python data science environments like Anaconda, or can be installed using pip:
```bash
pip install pandas matplotlib seaborn numpy
```

## Usage

1. **Ensure you have the data file:** The project expects a CSV file named `fcc-forum-pageviews.csv` in the specified path within the script (currently `C:/Users/Mehak/OneDrive/Documents/Ayaan/Data Science/fcc-forum-pageviews.csv`). You might need to update this path.
2. **Run the Jupyter Notebook:** Open and run the `fcc.ipynb` notebook in a Jupyter environment.
   Alternatively, you can convert the notebook to a Python script and run it.

The script will perform the data loading, cleaning, and then generate and save the three plots mentioned above. It will also display the plots if run in an environment that supports matplotlib's interactive mode.

## Data Source

The data used is from the freeCodeCamp forum page views, provided in a CSV file format. The expected columns are `date` (parsable as datetime) and `value` (page views).

## Example Output

The script will output:
- Basic statistics about the cleaned data (data shape, date range, page view range).
- Saved image files: `line_plot.png`, `bar_plot.png`, `box_plot.png`.
- Displayed plots (if in an interactive environment).
- Basic statistics derived from the analysis (total data points, average/median daily page views, standard deviation).

## Contribution

Feel free to fork this repository and contribute by:
- Improving the visualizations.
- Adding more analyses.
- Enhancing the data cleaning process.
- Optimizing the code.

Please open an issue to discuss any major changes.
