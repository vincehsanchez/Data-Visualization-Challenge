# Data-Visualization_Challenge
1. Compare the performance of drug of interest, Capomulin, against the other treatment regimens.
2. Generate all of the tables and figures needed for the technical report of the clinical study. 
3. Write top-level summary of the study results.

### Prepare the Data
Run and merge DataFrames into a single DataFrame.

Display data, and remove duplicate time points.

Display the data with removed timepoints.

Use this cleaned DataFrame for the remaining steps.

Display the updated number of unique mice IDs.

### Generate Summary Statistics
Create a DataFrame of summary statistics.
1. A row for each drug regimen.
2. A column for each of the following statistics of tumor volume:
- mean
- median
- variance
- standard deviation
- SEM

### Create Bar Charts and Pie Charts
Generate two bar charts show the total number of rows for each drug regimen and two pie charts that show the distribution of female versus male mice.
- Create the first chart with the Pandas DataFrame.plot() method and second one with Matplotlib's pyplot methods.


### Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 
Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
Determine outliers by using the upper and lower bounds, and then print the results.
Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.
hint: All four box plots should be within the same figure. Use this Matplotlib documentation page Links to an external site. for help with changing the style of the outliers.

### Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin.

Generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot:
- Mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

### Calculate Correlation and Regression
Calculate between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen:
1. correlation coefficient
2. linear regression model 
3. Plot the linear regression model on top of the previous scatter plot.
