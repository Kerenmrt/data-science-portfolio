# Life Expectancy Analysis using Multiple Linear Regression

## Project Overview
This project analyzes the influence of socio-economic factors on life expectancy in districts and cities of West Sumatra Province in 2022. The study focuses on understanding how poverty depth, employment rate, and net income affect life expectancy at birth using a Multiple Linear Regression approach.

The analysis aims to identify key socio-economic variables that significantly influence life expectancy and provide insights that could support policy making in improving public welfare.

## Dataset
The dataset used in this study was obtained from the official website of the Central Bureau of Statistics (BPS) Indonesia.

Region: West Sumatra Province  
Year: 2022

Variables used in the analysis:

- Life Expectancy at Birth (Response Variable)
- Poverty Depth Index
- Percentage of Population Aged 15+ Who Are Employed
- Net Income

## Methodology

The analysis follows several stages:

1. Data exploration and descriptive statistics
2. Correlation analysis between variables
3. Data visualization using scatter plots
4. Classical assumption tests:
   - Normality Test
   - Multicollinearity Test
   - Homoscedasticity Test
   - Autocorrelation Test
5. Multiple Linear Regression modeling
6. Model evaluation using:
   - RMSE
   - MAE
   - R-squared

The analysis was conducted using the R programming language.

Libraries used:
- ggplot2
- corrplot
- lmtest
- lawstat
- nortest
- car
- dplyr

## Results

The regression analysis shows that:

- Poverty Depth Index has a significant negative effect on life expectancy.
- Net income has a significant positive effect on life expectancy.
- The employment variable does not show a significant effect.

Model performance:

- RMSE: 0.128
- MAE: 0.101
- R²: 0.5007

This indicates that approximately 50% of the variation in life expectancy can be explained by the variables used in the model.

## Infographic Summary

![Infographic](infographic-life-expectancy.jfif)

## Project Report

The full research report can be accessed below:

[Download Full Report](Life_Expectancy_Report.pdf)

## Tools Used
- R Programming
- Statistical Modeling
- Data Visualization
- Multiple Linear Regression

## Author
Keren Marito Lumban Gaol  
Data Science Student – Institut Teknologi Sumatera
