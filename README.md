# 🚗 Automobile Market Analysis

### Exploring Price, Performance and Popularity Trends in the US Car Market

A data-driven Exploratory Data Analysis (EDA) project analyzing automobile specifications, pricing, performance, fuel efficiency, popularity, and market trends using Python.

---

## 📌 Project Overview

This project analyzes a real-world automobile dataset to understand how vehicle specifications such as:

- Engine Horsepower
- Engine Cylinders
- Vehicle Size
- Fuel Type
- Transmission
- Drivetrain
- Vehicle Style
- Model Year

relate to **MSRP (Manufacturer's Suggested Retail Price)**.

The project follows a complete data analytics workflow — from data exploration and cleaning to statistical analysis, visualization, business insights, and recommendations.

The original dataset contained **11,914 records and 16 columns**. After removing **715 duplicate records** and handling missing values, the final analysis-ready dataset contains **11,199 unique vehicle listings**. :contentReference[oaicite:1]{index=1}

---

## 🎯 Project Objectives

- Understand the structure and characteristics of the automobile dataset.
- Clean missing values, duplicate records, and inconsistent data.
- Perform descriptive statistical analysis.
- Conduct univariate analysis of numerical and categorical variables.
- Analyze relationships between vehicle specifications and MSRP.
- Identify the strongest factors associated with vehicle pricing.
- Study market popularity across manufacturers and vehicle styles.
- Analyze fuel-efficiency and drivetrain patterns.
- Create meaningful data visualizations.
- Translate analytical findings into business insights.
- Provide practical recommendations for automobile manufacturers, dealers, and marketers.

---

## 📊 Dataset

### Dataset Information

| Attribute | Details |
|---|---|
| Dataset | Automobile Specifications & Pricing Dataset |
| Original Records | 11,914 |
| Final Records | 11,199 |
| Duplicate Rows Removed | 715 |
| Columns | 16 |
| Time Period | 1990–2017 |
| Manufacturers | 48 |
| Distinct Models | 915 |
| Target Variable | MSRP |

The dataset is based on a public car-listings dataset and was provided as `cleaned_dataset.csv`. :contentReference[oaicite:2]{index=2}

### Main Features

| Feature | Description |
|---|---|
| `Make` | Vehicle manufacturer |
| `Model` | Vehicle model |
| `Year` | Model year |
| `Engine Fuel Type` | Fuel used by the vehicle |
| `Engine HP` | Engine horsepower |
| `Engine Cylinders` | Number of engine cylinders |
| `Transmission Type` | Automatic, Manual, etc. |
| `Driven_Wheels` | Front, Rear, All, Four-wheel drive |
| `Number of Doors` | Number of vehicle doors |
| `Market Category` | Luxury, Performance, Crossover, etc. |
| `Vehicle Size` | Compact, Midsize, Large |
| `Vehicle Style` | Sedan, SUV, Coupe, etc. |
| `highway MPG` | Highway fuel efficiency |
| `city mpg` | City fuel efficiency |
| `Popularity` | Popularity score |
| `MSRP` | Manufacturer's Suggested Retail Price |

---

# 🧹 Data Cleaning

Several data-quality issues were identified and addressed before analysis.

### Duplicate Records

- Original records: **11,914**
- Duplicate records removed: **715**
- Final records: **11,199**

Duplicate rows were removed using:

```python
df.drop_duplicates()
