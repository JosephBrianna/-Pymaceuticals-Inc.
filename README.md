# README for Pymaceuticals Inc.

---

## Overview
This project is aimed at analyzing the effectiveness of various drug regimens on tumor development in mice. Specifically, the focus is on comparing "Capomulin", "Ramicane", "Infubinol", and "Ceftamin" drug regimens.

## Contents

### Dependencies and Setup
This script requires:
- matplotlib: For creating visual plots.
- pandas: For data manipulation and analysis.
- scipy.stats: For statistical functions like Pearson correlation and linear regression.
- IPython.display: To display data tables.

### Data Files
- Mouse_metadata.csv: Contains metadata about the mice.
- Study_results.csv: Contains study results of the drug trials on the mice.

### Merging Data
The script reads in data from two CSV files and merges them based on the "Mouse ID" to get a comprehensive view.

### Data Cleaning
It identifies any duplicated data based on "Mouse ID" and "Timepoint" and then filters the data to remove these duplicates, creating a clean dataset for analysis.

### Summary Statistics
The script computes various statistics related to the "Tumor Volume (mm3)" for each drug regimen. It calculates the mean, median, variance, standard deviation, and SEM of the tumor volume.

### Bar and Pie Charts
- Bar Charts: The script produces two bar charts (one using pandas and one using pyplot) that display the number of rows (i.e., the number of mice/timepoints) for each drug regimen.
  
- Pie Charts: Two pie charts are plotted to visualize the distribution of male vs. female mice in the study.

### Quartiles, Outliers, and Boxplots
For each of the specified drug treatments ("Capomulin", "Ramicane", "Infubinol", "Ceftamin"), the script:
- Identifies the last (maximum) timepoint for each mouse.
- Determines the tumor volume at this last timepoint.
- Identifies any potential outliers in the tumor volumes.
- Visualizes the tumor volumes using a boxplot.

### Line and Scatter Plots
- Line Plot: The script selects one mouse treated with Capomulin and plots its tumor volume over time.
  
- Scatter Plot: For mice treated with Capomulin, the script creates a scatter plot of mouse weight versus average tumor volume.

### Correlation and Regression
Finally, the script determines the correlation between mouse weight and average tumor volume for the Capomulin regimen and visualizes this relationship using a scatter plot with a linear regression model.

## Analysis
- Add your specific findings and analysis here.

---

## Usage
To run the script, make sure you have all the required dependencies installed. Then, simply execute the Python script. Ensure that the data files (`Mouse_metadata.csv` and `Study_results.csv`) are placed in the `data/` directory or modify the paths accordingly.

---

## Additional Notes
When using this script, always ensure that the data files are up-to-date and haven't been corrupted or modified in a way that could affect the accuracy of the analysis.

---

## Contributing
To contribute to this project, please fork the repository, make your updates and then create a pull request. Ensure that any new functionalities added are well-documented and tested.

---

## License
This project is licensed under the MIT License.for personal and educational use only 
