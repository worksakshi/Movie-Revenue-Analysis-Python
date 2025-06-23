# Movies Revenue Analysis Python

## Project Overview

**Project Title**: Movies Revenue Analysis  
**Datasource** : movies.csv

This project analyzes a dataset of movies to uncover insights into what factors influence a movie’s gross revenue. We explore relationships between budget, votes, ratings, genre, and time to identify trends and drivers of box office performance.

## Objectives

1. Clean and preprocess the movie dataset
2. Analyze correlations between numerical and categorical features
3. Identify key drivers of high gross revenue
4. Detect outliers and skewness in budget and revenue
5. Explore trends over time (e.g., budget growth)
6. Visualize top-performing directors and genres

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

#### 5. Ratings and Revenue
PG-13 and PG rated movies generate the highest median revenue.

Broader audience appeal = higher returns.

#### 6. Budget Trend Over Time
Median budgets remained fairly constant from 1980–2020.

Spikes observed between 1997 and 2013.

#### 7. Top Performing Directors and Genres
Directors and genres ranked by median gross revenue.

Barplots highlight top 10 in each category.














