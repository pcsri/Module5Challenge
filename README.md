What good is data without a compelling plot to tell its story?

In this assignment, you’ll use your knowledge of Matplotlib to analyze a real-world dataset.

Background
You've just joined Pymaceuticals, Inc., a pharmaceutical company specializing in anti-cancer medications. The company is currently screening for potential treatments for squamous cell carcinoma (SCC), a common form of skin cancer.

As a senior data analyst, you have access to the complete data from a recent animal study. In this study, 249 mice with SCC tumors were treated with various drug regimens. Tumor development was observed and measured over 45 days. The aim was to compare the efficacy of Pymaceuticals’ drug of interest, Capomulin, against other treatment regimens.

The executive team has tasked you with generating all the tables and figures for the technical report of the clinical study. They have also requested a top-level summary of the study results.

Module 5 Challenge files (Links to an external site).
Instructions
This assignment consists of the following tasks:

Prepare the Data

Run the provided package dependency and data imports.
Merge the mouse_metadata and study_results DataFrames into a single DataFrame.
Display the number of unique mouse IDs in the data.
Check for any mouse ID with duplicate time points, display the data, and create a new DataFrame excluding this data. Use this cleaned DataFrame for the remaining steps.
Display the updated number of unique mouse IDs.

Generate Summary Statistics

Create a DataFrame of summary statistics.
Include a row for each drug regimen with columns for mean, median, variance, standard deviation, and SEM of the tumor volume.

Create Bar Charts and Pie Charts

Generate two identical bar charts showing the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study. Create the first bar chart with the Pandas DataFrame.plot() method and the second with Matplotlib's pyplot methods.
Generate two identical pie charts showing the distribution of female versus male mice in the study. Create the first pie chart with the Pandas DataFrame.plot() method and the second with Matplotlib's pyplot methods.
Calculate Quartiles, Find Outliers, and Create a Box Plot

Calculate the final tumor volume of each mouse across four promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
Calculate the quartiles and IQR, and determine potential outliers.
Create a grouped DataFrame showing the last time point for each mouse, merge it with the cleaned DataFrame.
Create lists for treatment names and tumor volume data.
Loop through each drug in the treatment list, locate the corresponding rows, and append the final tumor volumes to the list.
Determine outliers using upper and lower bounds, then print the results.
Generate a box plot showing the distribution of the final tumor volume for all mice in each treatment group, highlighting any potential outliers.

Create a Line Plot and a Scatter Plot

Select a single mouse treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

Calculate Correlation and Regression

Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the Capomulin treatment regimen.
Plot the linear regression model on top of the previous scatter plot.