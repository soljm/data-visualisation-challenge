# Pymaceuticals Inc.
From Module 5: Data Visualisation from the Data Analytics Boot Camp by Monash University and EdX.

By implementing skills learnt throughout the module, an attempt at the challenge has been submitted here.

## Contents
- `.ipynb` file with the main code
- Two CSV files given as resources

## Explanation
Most of the code is self-explanatory and commented. Below are a few points on some differences to the starter code given. A title and labels were added for each graph to provide clarity.
### Calculate Quartiles, Find Outliers, & Create a Box Plot
`.groupby()` was used to group the dataset by **Mouse ID** and **Timepoint**, and `.max()` was applied to find the last timepoint for each mouse. This was then merged into the original DataFrame. `.isin` was used to filter the DataFrame to only include the necessary drug regimens.
### Create a Line Plot & a Scatter Plot
Filtered the merged DataFrame to only contain data for **Capomulin**. `.iloc()` was used to grab the **Mouse ID** of the first mouse after the DataFrame was filtered. A line graph was created from this value/data.

## Credits
Credits to my friend, NT, who gave me pointers on the following:
- Using `.isin()` to filter the necessary drug regimens
- Grabbing the mouse ID of the first mouse using `.iloc[0]` to graph a single mouse
- Consolidating messy/long codes