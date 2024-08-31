# phase3-project
# Predicting waterWells conditions in Tanzania
## Business Understanding
### Problem Statement

The lack of clean and potable water is a significant problem in many Tanzanian communities. To combat this, the Tanzanian Ministry of Water has installed numerous water wells nationwide. However, many of these wells are not functioning properly, limiting access to clean water.

This project aims to develop a predictive model using data from Taarifa and the Tanzanian Ministry of Water to assess the condition of water wells, identifying which pumps are functional, need repairs, or are non-functional. The goal is to enhance maintenance efforts and ensure reliable access to clean water for communities across Tanzania.

### Research Question
Which classifier model can accurately predict the condition of water wells in Tanzania?

### Objectives

#### Main Objective
To predict the condition of water wells in Tanzania to ensure that clean and potable water is available to communities across Tanzania

#### Specific Objective 
To understand the problem statement and the goal of the project

To identify the variables that can impact the functionality of water wells

To determine the target variable (functional, need repairs, or non-functional)

### Metric of Success
The model will be considered a success when both accuracy and f1 score are between 0.8 to 1

## 2.  Data  Understanding
###Data Description
amount_tsh - Total static head (amount water available to waterpoint)

date_recorded - The date the row was entered

funder - Who funded the well

gps_height - Altitude of the well

installer - Organization that installed the well

longitude - GPS coordinate

latitude - GPS coordinate

wpt_name - Name of the waterpoint if there is one

basin - Geographic water basin

subvillage - Geographic location

region - Geographic location

region_code - Geographic location (coded)

district_code - Geographic location (coded)

lga - Geographic location

ward - Geographic location

population - Population around the well

public_meeting - True/False

recorded_by - Group entering this row of data

scheme_management - Who operates the waterpoint

scheme_name - Who operates the waterpoint

permit - If the waterpoint is permitted

construction_year - Year the waterpoint was constructed

extraction_type - The kind of extraction the waterpoint uses

extraction_type_group - The kind of extraction the waterpoint uses

extraction_type_class - The kind of extraction the waterpoint uses

management - How the waterpoint is managed

management_group - How the waterpoint is managed

payment - What the water costs

payment_type - What the water costs

water_quality - The quality of the water

quality_group - The quality of the water

quantity - The quantity of water

quantity_group - The quantity of water

source - The source of the water

source_type - The source of the water

source_class - The source of the water

waterpoint_type - The kind of waterpoint

waterpoint_type_group - The kind of waterpoint

## 3.Data Preparation
Uniformity - Handling Missing Values

Consistency - Encoding Categorical Variables

Completeness - Ensure the dataset has no missing values

Scaling

Handling Class Imbalance

Uniformity - Handling Missing Values

## 4.Modeling
The Random Forest Classifier model has an accuracy of 0.8168 and an F1 score of 0.8097

In terms of accuracy, the random forest classifier has a higher accuracy score of 0.81 compared to the other 2 models, which had accuracy scores of  0.75 (decision tree), and 0.65 (logistic regression).

In terms of the F1 score, the random forest classifier has a higher F1 score of 0.81 compared to the other 2 models, which had F1 scores of 0.76 (decision tree), and 0.62 (logistic regression).

Based on these results, the random forest classifier appears to be performing the best among the 3 models.

Hyperparameter tuning and cross-validation is performed because they help to optimize the model performance and prevent overfitting or underfitting. The randomized search cross-validation helps to perform an efficient search for the optimal hyperparameters and cross-validate the model, which leads to better model performance and robustness.

The accuracy of the model is 0.8229, which means that the model correctly predicted the class label of 81.68% of the test data instances. The F1 score is 0.8097. A higher F1 score indicates a better performance of the model.

This tuned model has better performance metrics and hence a good model.

## 6.Conclusion and Recommendations
### Conclusion
The model could be further enhanced by incorporating additional data, particularly for the "functional needs repair" class, to address class imbalance issues.

### Recommendations
1.The Tanzania Ministry of Water should invest in better waterpoint types such communal standpipes and hand pumps

2.The Tanzania Ministry of Water should ensure that the extraction type for the wells is mostly through gravity and handpump

3.The Tanzania Ministry of Water should ensure that the gps height(altitude of the well) for most water points is high enough

4.The Tanzania Ministry of Water should also ensure that the people using the waterpoints pay either monthly, annually or per bucket to ensure that the wells are well maintained