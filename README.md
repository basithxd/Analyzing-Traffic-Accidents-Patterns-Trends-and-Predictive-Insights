# Analyzing-Traffic-Accidents-Patterns-Trends-and-Predictive-Insights
A working demo of simple analytical technique to answer 3 research questions

Subject: README.md – 2005–2014 UK Traffic Flow & Accident Analysis

# 2005–2014 UK Traffic Flow and Accident Analysis

## Overview

This repository contains an analytical and predictive study of road traffic accidents in **England, Scotland, and Wales** using official UK traffic and accident datasets spanning **2005–2014**. The project focuses on identifying patterns, trends, and predictive factors related to accident severity, casualties, police response, and time-of-day accident frequency.

The analysis is implemented primarily in **R**, using machine learning models such as **Random Forests** and **Ridge Regression**.

---

## Dataset

**Source:** UK Department for Transport
**Coverage:** 2005–2014
**Geography:** England, Scotland, Wales

### Key Data Files

* `accidents_2005_to_2007.csv`
* `accidents_2009_to_2011.csv`
* `accidents_2012_to_2014.csv`

These datasets are merged into a single dataframe for analysis.

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
* Urban vs Rural Area
* Police Attendance
* Date and Time of Accident

All categorical variables are properly factorized, and missing values are handled during preprocessing.

---

## Research Questions

1. **What factors best predict accident severity?**
2. **Can the number of casualties be predicted using road and environmental conditions?**
3. **How accurately can police response presence be forecasted?**
4. **What time of day experiences the highest accident frequency?**

---

## Methods

### Machine Learning Models

* Random Forest Classification (Accident Severity)
* Random Forest Regression (Casualties, Police Force)
* Ridge Regression (Casualty Prediction – Alternative Approach)

### Techniques Used

* Feature engineering
* Train-test splits
* Subsampling for scalability
* Variable importance analysis
* RMSE, R-squared, and accuracy metrics

---

## Results Summary

* **Accident Severity Prediction Accuracy:** ~84–85%
* **Casualty Prediction:** Limited explanatory power, indicating high randomness and external factors
* **Police Response Prediction:** Moderate error with stable RMSE
* **Time-of-Day Analysis:** Evening and afternoon periods show the highest accident frequencies

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
├── analysis/
│   ├── preprocessing.R
│   ├── severity_prediction.R
│   ├── casualty_prediction.R
│   └── time_of_day_analysis.R
├── results/
│   └── figures_and_outputs/
└── README.md
```

---

## How to Run

1. Install required R packages
2. Place CSV files in the `data/` directory
3. Run preprocessing scripts
4. Execute analysis scripts for each research question

---

## Use Cases

* Transportation safety analysis
* Urban planning and policy evaluation
* Machine learning applications in public safety
* Academic and educational projects

---

## License

This project is for **academic and educational purposes**. Dataset ownership remains with the UK Department for Transport.

---

## Authors


Basith M and Thanuja B 

---

If you want, I can also:

* Make this **shorter or more academic**
* Customize it for **Kaggle or coursework submission**
* Add **badges, citations, or data source links**
