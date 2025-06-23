# Movies Revenue Analysis Python

## Project Overview

**Project Title**: Movies Revenue Analysis  
**Datasource** : movies.csv

This project analyzes a dataset of movies to uncover insights into what factors influence a movie’s gross revenue. We explore relationships between budget, votes, ratings, genre, and time to identify trends and drivers of box office performance.

## Objectives

1. How votes and budget impact revenue.

2. Whether movie ratings influence earnings.
   
3. Trends in movie budget over time.
   
4. Which genres and directors generate the most revenue?

## Libraries Used
```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

## Project Structure

### A) Data Cleaning Steps:
1. Filled missing rating values with the mode
2. Filled missing budget with median
3. Dropped rows with remaining missing values
4. Removed duplicate movie entries based on name
5. Extracted Released Year from released column
6. Converted categorical columns to numeric codes for correlation analysis

### B) Exploratory Data Analysis (EDA)
#### 1. Distribution of Budget
Highly right-skewed; most movies operate with smaller budgets.

Visualized using KDE plot.



#### 2. Correlation Analysis
Strong positive correlation between:
. votes and gross (0.63)
. budget and gross (0.74)

Heatmaps created for both numerical and encoded features.

#### 3. Regression Analysis
Plots show positive trends between:

Budget and Gross Revenue (weaker slope)

Votes and Gross Revenue (sharper slope)

#### 4. Gross Revenue Distribution
Right-skewed: most movies earn less, a few earn extremely high.

Outliers identified using boxplot.

### C)  Exploratory Data Analysis (EDA)

## 1️⃣ Does Budget and Votes Affect Gross Revenue?

![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/budget_votes_vs_gross_comparison.png)

##### Insight:

As votes increase, gross revenue rises more sharply.

As budget increases, revenue also rises but more gradually.

##### Conclusion:
While budget and votes are the two most important factors influencing gross revenue, this pattern does not apply to all movies because the data is skewed. Just spending more or getting more votes doesn’t guarantee success for every film.










