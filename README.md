# A/B Testing using Machine Learning

## Introduction

This project applies Machine Learning (ML) to the robust methodology of A/B Testing, offering a step-by-step guide to improving digital marketing decisions through data science.

### Motivation

A/B Testing is a powerful strategy to validate changes in user interfaces and marketing strategies. By employing ML, we aim to account for the complexity of user behavior which traditional statistical methods may oversimplify. The end goal is to maximize user engagement and sales by understanding and leveraging the nuances of customer interactions.

### About the Project

Traditional A/B tests often fall short in painting the full picture due to their binary nature—focusing solely on the treatment and control groups' outcomes. This project aims to capture the multifaceted aspects of customer behavior by implementing an ML approach to A/B Testing, providing deeper insights into what truly influences user decisions.

#### Experiment: "Free Trial" Screener

Udacity conducted an experiment asking students how much time they could dedicate to a course. The responses were used to guide the students through the enrollment process, with the intention of setting clear expectations and reducing trial abandonment due to time constraints.

#### Project Goal

The analysis will identify which features contribute to enrollments and the effect of the "Setting Expectations" form on student enrollment figures.

The users that experience the form will be denoted as “Experiment = 1” The control group (users that don’t see the form) will be denoted as “Experiment = 0”.


## Data

The dataset includes 37 daily observations across the following columns:

- `Date`: Day, month, and day of the month.
- `Pageviews`: Total page views per day.
- `Clicks`: Total clicks per day for the given page.
- `Enrollments`: Daily enrollment numbers.
- `Payments`: Daily payment counts.

### Missing Data and Preprocessing

We address missing data, incorrect formatting, and prepare the dataset for ML modeling. This includes:

- Combining control and experiment data with identifiers.
- Creating a "Day of Week" feature.
- Dropping irrelevant columns and handling missing values.
- Shuffling data for unbiased learning.

## Machine Learning Models

We will test the following algorithms:

- Linear Regression
- Decision Trees
- XGBoost

### Dependencies

- Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn
- XGBoost
- Statsmodels

### Usage

The Jupyter Notebook is structured to guide you through four main tasks:

1. Loading the data.
2. Performing exploratory data analysis.
3. Preprocessing the data for modeling.
4. Building and evaluating ML models.

Instructions for setting up, executing the analysis, and contributing to the project are outlined below.

## Running the Analysis
To run the analysis, navigate to the notebook directory and launch the Jupyter notebook:
```bash
jupyter notebook AB_Testing_using_ML.ipynb

