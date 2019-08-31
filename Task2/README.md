# B. Synthetic Data

![badge](https://img.shields.io/badge/language-python-blue.svg)

>Either create from scratch, crawl or download a dataset of your choice and apply a machine learning method to extract information from the dataset. Examples could be a regression, classification or clustering analysis. 

Here I have decided to work on a classification project on Personal Injury Car Accidents. The *CarAccidentsPredictions.ipynb* notebook contains the data cleaning, exploratory analysis, ML models and results.

# :books: Table of content

- [Context](#car-Context)
- [Dataset](#fuelpump-Dataset)
- [Goal](#white_check_mark-Goal)
- [Evaluation](#chart_with_upwards_trend-Evaluation)
- [Target](#dart-Target)
- [Data Fields](#round_pushpin-Explanatory-Variables)
- [Results](#rocket-Results)
- [Synthetic Data](#robot-Synthetic-Data)

# :car: Context
For each personal injury accident (i.e. an accident occurring on a road open to public traffic, involving at least one vehicle and resulting in at least one victim requiring treatment), information describing the accident is entered by the police unit that intervened at the accident site. These entries are collected in the national road traffic injury file.

The present database lists all traffic accidents that occurred during a given year in metropolitan France and the overseas departments (Guadeloupe, French Guiana, Martinique, Reunion Island and Mayotte) with a simplified description. This includes information on the location of the accident, such as information on the characteristics of the accident and its location, the vehicles involved and their victims.

# :fuelpump: Dataset
The dataset contains thousands of individuals and 32 variables (which are either quantitative or categorical) with many missing values. The description of these variables is available in the file description.txt.

## File descriptions
- Xtrain.csv: matrix of input data for training (each individual is a row);
- ytrain.csv: vector of input targets for training (it has as many rows as Xtrain.csv);
- Xtest.csv: matrix of input data for prediction (each individual is a row);
- description.txt: description of variables.

# :white_check_mark: Goal
The objective is to predict the severity of a personal injury accident based on 31 descriptive variables. This probelm is traited as a classification problem.
NB: Here a regression approach could also have been considered.


# :chart_with_upwards_trend: Evaluation

The evaluation metric is the categorization accuracy (i.e. the usual classification score).


# :dart: Target
The target is the severity of each personal injury accident. It can take four different values:

1. Unscathed
2. Slight injury
3. Injured in hospital
4. Killed

# :round_pushpin: Explanatory Variables
See the file description.txt for a detailed description.

- month: Month of the accident
- day: Day of the accident
- time: Hours and minutes of the accident
- light: Lighting conditions in which the accident occurred.
- location: Location
- intersection: Intersection
- atmosphere: Weather conditions
- collision: Type of collision
- municipality: The municipality number is a code given by INSEE. The code has 3 digits on the right.
- department: INSEE code (Institut National de la Statistique et des Etudes Economiques) of the monitoring department.
- road: Road category
- traffic: Traffic regime
- nblanes: Total number of lanes of traffic
- reslane: Indicates the existence of a reserved lane, regardless of whether or not the accident occurs on that lane
- laneprofile: Long profile describes the gradient of the road at the accident site
- plan: Drawing in plan
- surface: Surface condition
- user: User category
- sex: Gender of the user
- route: Reason for travel at the time of the accident
- pedlocation: Pedestrian location
- pedaction: Pedestrian action
- pedcondition: This variable is used to specify whether the injured pedestrian was alone or not
- birth: User's year of birth
- dirtraffic: Direction of traffic
- catvehicle: Vehicle category
- nboccupants: Number of occupants in public transit
- obstacle: Fixed obstacle hit
- movobstacle: Mobile obstacle hit
- impact: Initial shock point
- maneuver: Main manoeuvre before the accident


# :rocket: Results
For each model tested, a summary table displays the results given by the algorithms. The metric used is the accuracy (ie. the number of correctly classified values). Other metrics could have been used (Specificity, Sensitivity, Recall, AUC/ROC curves). Here it seems that XGBoost performed best. (see mean_test_score in the tables)


# :robot: Synthetic Data

> Now derive a synthetic dataset, that shares as much information as possible with the original one regarding the machine learning process you applied; but is otherwise fundamentally different. How would you assess the quality of your data synthesis process?

Why synthetic data in this case?
- Test the ML process robustness to noise.
- Simulate not yet encountered conditions.
- Protect the privacy and confidentiality of authentic data. 
- Over sampling the minor class in case of imbalanced dataset.

Assumptions & Methods: 
- The out-of-sample data must reflect the distributions satisfied by the sample data.
- Replicate all important statistical properties: The assumption is that the true mean and standard deviation of each feature/category pair is known. In reality, if the synthetic data was too far off from these values, it could severely impact the accuracy of the trained model.
- Thus, I would use SMOTE (Synthetic Minority Over-sampling) technique to generate new synthetic samples and deal with my imbalanced classes in the training dataset.
- SMOTE is based on a KNN approach to select similar records and alter that record one column at a time.
