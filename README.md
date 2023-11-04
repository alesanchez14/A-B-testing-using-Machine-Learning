# A/B Testing using Machine Learning

## Introduction

This project bridges the gap between traditional A/B Testing and Machine Learning (ML) to refine digital marketing decisions. We present a step-by-step guide on utilizing data science to enhance the understanding and effectiveness of A/B Testing.

### Motivation

A/B Testing is instrumental in optimizing user interfaces and marketing tactics. Our approach enriches this testing with ML to embrace the intricate patterns of user behavior that standard statistical methods may not fully capture. We seek to bolster user engagement and increase sales by exploiting the subtle dynamics of customer interactions.

### About the Project

This initiative addresses the shortcomings of conventional A/B tests by incorporating an ML perspective. We strive to unravel the complex dimensions of customer behavior to provide a rounded view of the factors influencing user choices.

#### Experiment: "Free Trial" Screener

In the experiment, Udacity tested a change where if the student clicked “start free trial”, they were asked how much time they had available to devote to the course.

If the student indicated 5 or more hours per week, they would be taken through the checkout process as usual. If they indicated fewer than 5 hours per week, a message would appear indicating that Udacity courses usually require a greater time commitment for successful completion.

Why Implement the Form?

The goal with this popup was that this might set clearer expectations for students upfront, thus reducing the number of frustrated students who left the free trial because they didn’t have enough time.

However, what Udacity wants to avoid is “significantly” reducing the number of students that continue past the free trial and eventually complete the course

#### Project Goal

Our analysis focuses on pinpointing the key attributes that influence course enrollments and assessing the impact of the "Setting Expectations" form on student signup rates.

Designations within the data are as follows:
- “Experiment = 1” for users who encountered the form.
- “Experiment = 0” for users in the control group who did not.

## Data

The data spans 37 days and includes metrics such as:

- `Date`: The specific day's date.
- `Pageviews`: The count of page views each day.
- `Clicks`: The total daily clicks for the specified page.
- `Enrollments`: The number of enrollments per day.
- `Payments`: The count of daily payments.

### Missing Data and Preprocessing

Our preprocessing steps resolve issues with data quality and readiness for ML analysis, ensuring:

- Merging of control and experimental data with clear identifiers.
- Introduction of a "Day of Week" feature to capture temporal patterns.
- Exclusion of extraneous columns and resolution of missing values.
- Randomization of data to promote model generalizability.

## Machine Learning Models

We evaluate the performance of the following models:

- Linear Regression
- Decision Trees
- XGBoost

## Key Steps

The project encompasses these core phases:

- **Data Loading and Preprocessing**: Setting up the data for ML application.
- **Exploratory Data Analysis**: Visualizing and understanding data traits.
- **Feature Engineering**: Crafting features that can better inform model predictions.
- **Model Training and Evaluation**: Applying ML algorithms and assessing their predictive prowess.

## Prerequisites

Engage with this project equipped with:

- A working knowledge of Python.
- Familiarity with `pandas`, `scikit-learn`, and statistical concepts.

## Setup

Prepare your environment with these libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`
- `statsmodels`

## Usage

The provided Jupyter Notebook details each analysis step, enabling replication or adaptation for your datasets. Follow these steps to start:

1. Data acquisition.
2. Preliminary data inspection.
3. Data preparation for model fitting.
4. Model building and validation.

## Running the Analysis

Execute the analysis by launching the Jupyter notebook within the notebook's directory:

  ```bash
  jupyter notebook AB_Testing_using_ML.ipynb
```

## Conclusion

This project serves as a comprehensive guide for integrating ML into A/B testing frameworks. It demonstrates how ML can be applied to real-world business problems, providing a more nuanced understanding of user behavior and driving more effective business strategies.

