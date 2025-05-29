# NBA Player Statistics Analysis Project

## Project Overview

For this final project, I've analyzed a dataset of NBA player statistics using Python. My goal was to practice and demonstrate data cleaning, statistical analysis, and visualization skills. I used libraries like Pandas for data handling, NumPy, SciPy, and Statsmodels for the analysis, and Matplotlib and Seaborn for creating the plots.

## Meeting Project Requirements

This project directly addresses all the criteria outlined in the assignment:

* **Unique Dataset:** I used a unique NBA player statistics dataset for this analysis.
* **Sufficient Data Points:** After cleaning, my dataset ended up with 303 data points, which is well above the required minimum of 100.
* **Correlation Analysis:** I performed a correlation analysis between 'Minutes Played (MP)' and 'Win Shares (WS)'. I made sure these variables weren't directly dependent in the way the assignment cautioned against.
* **Multiple Visualizations:** Besides the correlation plot, I created two other distinct visualizations to explore different aspects of the data.
* **Data Cleaning:** I identified and handled all null values in the dataset.
* **Data Processing & Analysis:** I used various operations from NumPy, SciPy, and Statsmodels to process and analyze the data.
* **Visualizations:** I generated clear and informative plots to show data distributions and relationships.
* **Correlation Plot:** I included a scatter plot with a regression line for my correlation analysis.

## About the Dataset

The dataset I worked with is named `NBA FINAL CAPSTONE_UTF8.csv`. It contains various statistics for NBA players, including:
* `Rk` (Player Rank)
* `Player` (Player Name)
* `Age` (Player's Age)
* `Team` (Team Abbreviation)
* `Pos` (Player's Primary Position)
* `G` (Games Played)
* `MP` (Minutes Played)
* `PER` (Player Efficiency Rating)
* `TS%` (True Shooting Percentage)
* `WS` (Win Shares)
* And many other advanced performance metrics.

## My Approach (Methodology)

Here's how I went about analyzing the data:

1.  **Loading the Data:** First, I loaded the `NBA FINAL CAPSTONE_UTF8.csv` file into a Pandas DataFrame.
2.  **Cleaning the Data:**
    * I noticed that the 'Awards' column was completely empty (all null values), so I removed it from the dataset.
    * After that, I double-checked and confirmed there were no other missing values anywhere else.
    * This left me with 303 usable rows for my analysis.
3.  **NumPy Operations:** I used NumPy to perform several operations, including calculating the mean, standard deviation, maximum, and median of various numerical columns like 'MP', 'WS', 'PER', 'Age', and 'G'. I also counted players based on a specific condition.
4.  **SciPy Operation:** For a statistical test, I performed an independent t-test. I compared 'Minutes Played' between two groups of players: those with a high Player Efficiency Rating (above the median) and those with a lower rating.
5.  **Statsmodels Operation:** I built an Ordinary Least Squares (OLS) linear regression model. I used 'Win Shares' as my dependent variable and 'Minutes Played' as my independent variable to see how they relate.
6.  **Creating Visualizations:**
    * I made a histogram (with a Kernel Density Estimate) to show the distribution of 'Player Efficiency Rating'.
    * I also created a bar plot that displays the average 'Win Shares' for the top 5 player positions.
7.  **Correlation Analysis:** Finally, I generated a scatter plot with a regression line to visualize the relationship between 'Minutes Played' and 'Win Shares'. I also calculated and displayed their correlation coefficient.

## Key Findings

Through this analysis, I found:

* My dataset was successfully cleaned and had plenty of data points (303) for a thorough analysis.
* There's a clear positive correlation between 'Minutes Played' and 'Win Shares', which makes sense: the more a player plays, the more impact they generally have on their team's wins.
* My statistical tests showed a significant difference in minutes played between highly efficient players and less efficient ones.
* The visualizations effectively showed how player efficiency is distributed and which positions tend to contribute more in terms of 'Win Shares'.

