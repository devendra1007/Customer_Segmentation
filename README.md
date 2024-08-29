# Customer Data Analysis

## Project Overview

This project is designed to analyze customer data using R, focusing on exploratory data analysis, visualization, and k-means clustering. The dataset used is `Mall_Customers.csv`, which contains information about customers, including their gender, age, annual income, and spending score. The analysis includes summary statistics, visualizations, and the application of clustering techniques to identify customer segments.

## Requirements

- R version 4.0.0 or higher
- Required R libraries:
  - `readr`
  - `plotrix`
  - `ggplot2`
  - `purrr`
  - `NbClust`
  - `factoextra`

## Instructions

1. **Loading and Exploring the Data:**
   - The dataset is loaded using the `read.csv()` function.
   - Basic exploratory data analysis is performed using `head()`, `str()`, and `summary()` to get an overview of the data.
   - The columns are renamed for better readability, and summary statistics such as standard deviation for `Age`, `Annual Income`, and `Spending Score` are calculated.

2. **Visualizations:**
   - **Gender Distribution:**
     - A bar plot is created to visualize the gender distribution of customers.
     - A 3D pie chart is plotted to show the gender ratio.
   - **Age Analysis:**
     - A histogram is used to display the distribution of age among customers.
     - A boxplot is used to provide a descriptive analysis of the age data.
   - **Annual Income Analysis:**
     - A histogram and a density plot are used to visualize the distribution of annual income.
   - **Spending Score Analysis:**
     - A boxplot and histogram are created to analyze the distribution of spending scores.

3. **K-Means Clustering:**
   - The `kmeans` algorithm is applied to segment customers based on `Age`, `Annual Income`, and `Spending Score`.
   - The total intra-cluster sum of squares is calculated for different values of `k` to determine the optimal number of clusters.
   - The `NbClust` and `factoextra` libraries are used to visualize the optimal number of clusters using the elbow method (wss) and silhouette method.

4. **K-Means Clustering Visualization:**
   - Principal Component Analysis (PCA) is performed to visualize the clusters in a 2D space.
   - A scatter plot is created using `ggplot2` to show the relationship between annual income and spending score, colored by cluster.
   - A final plot is generated to visualize the clusters using PCA.

## Output

- The final output includes visualizations and cluster analysis plots that provide insights into customer segments based on their spending behavior and income.
- The project demonstrates how to apply k-means clustering to customer data and interpret the results through visualization.

## Notes

- The optimal number of clusters was determined to be 5, based on the elbow method (wss).
- The analysis and visualizations are saved in an PDF file as the final output.

## Author

- **Name:** Sahil Thorat
- **Date:** July 25, 2024
