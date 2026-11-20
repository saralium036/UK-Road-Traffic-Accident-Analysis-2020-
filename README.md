## UK Road Traffic Accident Analysis (2020)

### Project Overview

Road traffic accidents remain a major public safety concern, resulting in loss of life, serious injuries and significant economic and social consequences.

This project analyses road traffic accident data for the United Kingdom in 2020, with the aim of identifying patterns and relationships in accident occurrences, understanding factors associated with accident severity, and exploring how data analysis and machine learning can contribute to road safety planning.

The analysis uses accident, vehicle and casualty records from the UK Department for Transport. It combines data preparation, exploratory data analysis, association rule mining, geographical clustering and machine learning classification.

### Project Objectives

The main objectives were to:

Examine patterns in road traffic accidents across different times, days and road users.

Investigate accident characteristics and their relationship with accident severity.

Explore geographical patterns in accidents within Humberside.

Identify associations between accident characteristics using association rule mining.

Apply machine learning techniques to classify accident severity.

Develop recommendations that could help inform road safety initiatives and policy decisions.

### Tools and Technologies

The project used the following tools and techniques:

Python – Data processing, analysis and modelling.

Pandas and NumPy – Data extraction, cleaning and manipulation.

SQLite – Storage and querying of accident-related datasets.

Matplotlib and Seaborn – Data visualisation.

Scikit-learn – Machine learning, clustering and model evaluation.

MLxtend – Association rule mining using the Apriori algorithm.

Jupyter Notebook – Development and documentation of the analysis.

### Dataset

The analysis used three related datasets:

Accident data: Information about road traffic accidents, including location, date, time, road conditions, weather and severity.

Vehicle data: Information about vehicles involved in reported accidents.

Casualty data: Information about casualties involved in the accidents.

The datasets were stored in an SQLite database. Records relating to 2020 were extracted and loaded into Pandas DataFrames for further processing and analysis.

Data source: UK Department for Transport – Road Safety Data.

### Methodology

#### 1. Data Extraction and Cleaning

The accident, vehicle and casualty tables were extracted from the SQLite database.

Data preparation involved:

Identifying and handling missing and invalid values.

Investigating records containing unknown or invalid entries.

Addressing missing geographical coordinates.

Reviewing road and junction characteristics.

Handling missing driver, casualty and vehicle information.

Examining unusual values and potential outliers.

Combining relevant information from the accident, vehicle and casualty datasets.

#### 2. Exploratory Data Analysis

Exploratory analysis was conducted to understand accident patterns and identify trends across different categories.

The analysis examined:

Accident frequency by time of day and day of the week.

Patterns in motorcycle accidents by engine capacity, time and day.

Pedestrian accident patterns.

Differences in accident characteristics across road users.

Some of the observations included:

Accident occurrences were highest around 6 pm.

Friday recorded a high number of accidents.

Pedestrian accidents showed noticeable peaks around 9 am and 4 pm.

Motorcycles with engine capacities of 125cc and below recorded a peak around 6–7 pm on Saturdays.

Motorcycles above 500cc recorded a peak around 5–6 pm on Mondays.

#### 3. Association Rule Mining

The Apriori algorithm was applied to identify relationships between accident characteristics and severity.

The analysis used the following thresholds:

Parameter

Threshold

Confidence

0.9

Lift

1.2

Support

0.5

The resulting association rules highlighted relationships between accident characteristics and casualty or accident severity. Several rules indicated associations with slight severity.

#### 4. Geographical Clustering

K-Means clustering was used to explore the geographical distribution of road traffic accidents in Humberside.

The elbow method was applied to help determine the number of clusters. Five clusters were selected, identifying accident concentration areas around:

Hull

Bridlington

Grimsby

Scunthorpe

Goole

A further clustering analysis explored relationships involving speed limits and weather conditions.

#### 5. Outlier Analysis

The Interquartile Range (IQR) method was used to investigate potential outliers in:

Driver age

Casualty age

Vehicle age

Unusual observations were reviewed, with plausible values retained rather than automatically removed.

#### 6. Machine Learning and Classification

Machine learning techniques were applied to explore the classification of road traffic accident severity.

The models and techniques included:

Decision Tree Classifier

K-Nearest Neighbours (KNN)

Naive Bayes

Logistic Regression

Stacking Classifier

Hyperparameter tuning and 10-fold cross-validation were also explored.

The reported model accuracy reached approximately 96% on the merged dataset.

Feature importance was examined to understand which variables contributed to the classification results.

#### Key Findings

The analysis provided several observations:

Accident occurrences varied across different times and days of the week, with evening periods and Fridays showing notable patterns.

Pedestrian accidents showed identifiable morning and afternoon peaks.

Motorcycle accident patterns differed according to engine capacity.

Geographical clustering identified five accident concentration areas within Humberside.

Association rule mining revealed relationships between selected accident characteristics and severity.

Machine learning provided a way to investigate the classification of accident severity using the available accident-related information.

### Recommendations

Based on the findings, the project proposed several measures that could contribute to improving road safety:

Improved public transportation: Encouraging the use of public transport could help reduce the number of private vehicles on the road.

Flexible and hybrid working arrangements: Reducing unnecessary commuting may help ease traffic congestion and exposure to road risks.

Speed monitoring: Greater use of speed cameras and enforcement measures could help address speeding-related risks.

Improved junction controls: Reviewing junction layouts and traffic control measures could help reduce accidents at high-risk locations.

### Project Limitations

The analysis was based on the available 2020 accident records. Some fields contained missing, invalid or unknown values, requiring data-cleaning and imputation approaches.

Certain estimated values were based on assumptions where direct information was unavailable. These assumptions may influence some analytical results.

The findings represent patterns and relationships within the dataset and should not automatically be interpreted as evidence of causation. The reported classification performance should also be considered in the context of the dataset, selected features and modelling approach.

### Conclusion

This project demonstrates the application of data analytics and machine learning to a public safety problem.

By combining data cleaning, exploratory analysis, association rule mining, geographical clustering and classification techniques, the study explored accident patterns, relationships between road safety factors and potential areas for intervention.

The project also demonstrates how data can be used to generate insights that may support evidence-informed road safety decisions and further investigation.

### Repository Contents

Big_Data_Project_10082023.ipynb – Jupyter Notebook containing the project analysis and code.

### Author

Sarah Ojo


