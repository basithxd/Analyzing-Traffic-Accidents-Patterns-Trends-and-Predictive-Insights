# Analyzing-Traffic-Accidents-Patterns-Trends-and-Predictive-Insights
A working demo of simple analytical technique to answer 3 research questions


# 2005–2014 UK Traffic Flow and Accident Analysis

## Overview

This repository contains an analytical and predictive study of road traffic accidents in **England, Scotland, and Wales** using official UK traffic and accident datasets spanning **2005–2014**. The project investigates patterns, trends, and predictive factors related to accident severity, casualties, police response, and time-of-day accident frequency.

All analysis is conducted within **a single notebook**, implemented primarily in **R**, using machine learning techniques such as **Random Forests** and **Ridge Regression**.

---

## Dataset

**Source:** UK Department for Transport
**Coverage:** 2005–2014
**Geography:** England, Scotland, Wales
**Link:** https://www.kaggle.com/datasets/daveianhickey/2000-16-traffic-flow-england-scotland-wales

### Data Files

* `accidents_2005_to_2007.csv`
* `accidents_2009_to_2011.csv`
* `accidents_2012_to_2014.csv`

The datasets are combined into one unified dataframe during preprocessing.

---

## Key Variables

* Accident Severity
* Number of Vehicles
* Number of Casualties
* Road Type
* Speed Limit
* Junction Control
* Pedestrian Crossing Controls
* Light Conditions
* Weather Conditions
* Road Surface Conditions
* Urban or Rural Area
* Police Attendance
* Date and Time of Accident

Categorical variables are converted to factors, and the dataset contains no missing values after cleaning.

---

## Research Questions

1. **Which factors are most predictive of accident severity?**
2. **Can road and environmental conditions predict the number of casualties?**
3. **How accurately can police attendance be forecasted?**
4. **What times of day experience the highest frequency of accidents?**

---

## Methods

### Models Used

* Random Forest Classification (Accident Severity)
* Random Forest Regression (Casualties, Police Force)
* Ridge Regression (Alternative casualty prediction approach)

### Analytical Techniques

* Data cleaning and feature engineering
* Train–test splits
* Subsampling for computational efficiency
* Variable importance analysis
* Performance metrics (Accuracy, RMSE, R-squared)

---

## Results Summary

* **Accident Severity Prediction Accuracy:** approximately 84–85%
* **Casualty Prediction:** low R-squared values, suggesting high variability and external influences
* **Police Response Prediction:** stable RMSE with moderate predictive accuracy
* **Time-of-Day Trends:** highest accident counts occur during afternoon and evening periods

---

## Libraries Used

```r
randomForest
caret
dplyr
ggplot2
lubridate
glmnet
vip
foreach
doParallel
```

---

## Repository Structure

```
├── data/
│   ├── accidents_2005_to_2007.csv
│   ├── accidents_2009_to_2011.csv
│   └── accidents_2012_to_2014.csv
├── analysis_notebook.Rmd  (or .ipynb / .R)
└── README.md
```

---

## How to Run

1. Install the required R packages
2. Place all CSV files in the `data/` directory
3. Open and run the analysis notebook from top to bottom

---

## Use Cases

* Traffic safety and risk analysis
* Urban planning and transportation policy
* Machine learning applications in public-sector data
* Academic and instructional use

---

## License

This project is intended for **academic and educational purposes only**. Dataset ownership remains with the UK Department for Transport.

---

## Authors
Basith M and Thanuja B
