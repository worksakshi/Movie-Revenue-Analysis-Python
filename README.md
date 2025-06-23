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
![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/Correlation%20Between%20Numerical%20Features.jpg)

To just not limit to numerical relationship, I have explored categorical relationship too.
![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/Gross%20Revenue%20Distribution.pnghttps://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/Correlation%20Between%20(Numerical%20%26%20Categorical)%20Features.jpg
)


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

#### Insight:

As votes increase, gross revenue rises more sharply.

As budget increases, revenue also rises but more gradually.

#### Conclusion:
While budget and votes are the two most important factors influencing gross revenue, this pattern does not apply to all movies because the data is skewed. Just spending more or getting more votes doesn’t guarantee success for every film.


## 2️⃣  Do Ratings Affect Movie Revenue?

![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/budget_votes_vs_gross_comparison.png)

#### Insight:
Movies with a PG-13 rating tend to generate the highest median revenue, followed by PG, G, and R.

#### Conclusion:
Ratings do have an impact. Films with broader audience appeal generally perform better financially than those with restrictive ratings.


## 3️⃣ Has Movie Budget Increased Over Time?

![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/budget_votes_vs_gross_comparison.png)

#### Insight:
From 1980 to 2020, there wasn't a consistent rise in movie budgets. However, noticeable spikes were observed between 1997 and 2013.

#### Conclusion:
Budgets have not grown linearly. The film industry has fluctuating investment trends depending on market cycles.


## 4️⃣ Which Genres or Directors Generate Higher Revenue?

![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/Top%2010%20High%20Performing%20Directors.png
)

![Insight_1](https://github.com/worksakshi/Movie-Revenue-Analysis-Python/blob/main/Top%2010%20High%20Performing%20Genre.png
)

#### Insight:
Specific directors and genres like Adventure, Action, and high-profile names show higher median gross revenues.

#### Conclusion:
Some creative teams consistently outperform in terms of revenue generation.









