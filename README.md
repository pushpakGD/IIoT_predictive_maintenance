# IIoT_predictive_maintenance

## General Information About The Project
- **Objective:** The primary objective of this project is to implement predictive maintenance for a milling machine using Industrial Internet of Things (IIoT) data.
- **Development Environment:** The project is developed in Python and structured as Jupyter Notebooks.
- **Dataset:** The project leverages a dataset collected from sensors and machine logs. This dataset aims to predict when maintenance is required to prevent unexpected breakdowns.
               This dataset was taken from UCI machine learning repository [https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset****].

## Project Goal:
It aims to forecast maintenance needs and identify potential types of failures associated with the milling machine.
The primary goal of this project is to develop a machine learning model that can utilize sensor data from the milling machine, based on Industrial Internet of Things (IIoT) technology.                      
Decision trees and the Random Forest classifier have been employed in this project to achieve these objectives.

##Results Obtained:
- Strong Correlations:
  The variables, including Process temperature, Air temperature, Torque, and Rotational speed, exhibit strong correlations.   This suggests that changes in one of these variables often coincide with changes in the others, indicating a potential      relationship between them.
- Common Causes of Machine Failure:
  Machine failures in this dataset are most frequently associated with Tool Wear, which is the leading cause. Torque and      Rotational Speed are the next significant contributors to machine failures. Understanding and monitoring these factors   
  could help in predicting and preventing failures.
- Feature Importance in Predictive Models:
  In both the Decision Tree and Random Forest models, Torque emerges as a crucial predictor for machine failures. It is 
  followed closely by Air Temperature. These features play a significant role in determining whether a machine failure is 
  likely.
- Model Comparison:
  When comparing the Decision Tree and Random Forest classifiers, it's evident that the Random Forest Classifier slightly 
  outperforms the Decision Tree model in terms of accuracy. This suggests that the ensemble approach used in Random Forest 
  helps improve predictive performance.
  
##Information about the dataset and the attribute:
The dataset consists infromation from an existing milling machine and consists of 10,000 data points from a stored as rows with 14 features in columns
- UID: unique identifier ranging from 1 to 10000
- product ID: consisting of a letter L, M, or H for low (50% of all products), medium (30%) and high (20%) as product quality variants and a variant-specific serial number
- type: the product type or variant. "L": Low-quality product variant, "M": Medium-quality product variant, "H": High-quality product variant
- air temperature [K]: generated using a random walk process later normalized to a standard deviation of 2 K around 300 K
- process temperature [K]: generated using a random walk process normalized to a standard deviation of 1 K, added to the air temperature plus 10 K.
- rotational speed [rpm]: calculated from a power of 2860 W, overlaid with a normally distributed noise
- torque [Nm]: torque values are normally distributed around 40 Nm with a SD = 10 Nm and no negative values.
- tool wear [min]: refers to the amount of wear and tear that a cutting tool used in the milling process has experienced over time.
- a 'machine failure' label that indicates, whether the machine has failed in this particular datapoint for any of the following failure modes are true.
    '1' indicates machine failure

