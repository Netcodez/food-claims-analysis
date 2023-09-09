# Food Claims Analysis
FoodClaimsAnalysis is a data analysis project that explores a dataset of food claims, performing data cleaning, visualization, and summary statistics to gain insights into claim characteristics and patterns.

## Food Claims Analysis
This repository contains the code and analysis for the Food Claims project, which focuses on analyzing and processing a dataset related to food claims. The project aims to perform data cleaning, exploratory data analysis, and visualization to gain insights into the food claims data.

## Table of Contents
- Introduction
- Dataset
- Data Cleaning
- Exploratory Data Analysis
- Conclusion
- Dependencies

### Introduction
Food claims refer to instances where individuals make claims related to food-related incidents, such as food poisoning or product quality issues. This project focuses on analyzing a dataset containing information about food claims, including the time to close a claim, the location of the incident, individuals involved, and the cause of the claim. The analysis aims to provide insights into various aspects of food claims and identify patterns or trends within the data.

### Dataset
The dataset used in this project consists of 2000 rows and 8 columns. The columns include:

- claim_id: Unique identifier for each claim (converted to string format)
- time_to_close: Time taken to close the claim in days (integer, discrete)
- location: Location of the incident (categorical)
- individuals_on_claim: Number of individuals involved in the claim (integer, discrete)
- cause: Cause of the claim (categorical)
- claim_amount: Amount claimed (float)
- amount_paid: Amount paid (float)
- linked_cases: Indicator for linked cases (boolean)

### Data Cleaning
During the data cleaning process, several actions were taken to ensure that the values in the dataset match the descriptions provided. These actions include:

- Converting the claim_id column from integer to string format.
- Regularizing the inconsistent casing in the cause column by converting all values to lowercase and replacing instances of "vegetables" with "vegetable."
- Converting the claim_amount column from a string datatype to a continuous datatype (float) and removing the currency symbol (R$) to regularize the values.
- Handling missing values by replacing them with appropriate values, such as replacing missing values in the amount_paid column with the median amount paid and missing values in the linked_cases column with the value False.

### Exploratory Data Analysis
The exploratory data analysis section includes various visualizations and analyses to gain insights into the food claims data. Some of the key findings include:

- The distribution of claims by location, with RECIFE having the highest number of claims.
- The time taken to close claims, including summary statistics such as mean, standard deviation, minimum, maximum, and quartiles.
- The relationship between time to close and location, explored through histograms, box plots, and scatter plots.
- Heatmap showcasing the average time to close claims across different locations.
  
### Conclusion
The Food Claims Analysis project provides valuable insights into food claims data, highlighting patterns, and trends related to claim closure time, location, and causes. The analysis can help stakeholders better understand and address food-related incidents, improve response times, and enhance overall customer satisfaction.

### Dependencies
The following dependencies are required to run the code:

- pandas
- matplotlib
- seaborn
- Install the dependencies using pip
