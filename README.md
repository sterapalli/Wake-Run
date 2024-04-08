# Walk-Run
Walk vs Run Classification using Sensor Data from iPhone 5c

**Overview**

This repository contains code for a classification task to differentiate between walking and running activities using sensor data collected from an iPhone 5c. The dataset consists of accelerometer and gyroscope readings from the device, along with metadata such as the date, time, user, and wrist where the device was placed.

The classification task involves predicting the activity type (walking or running) based on the sensor data and other features provided.

**Dataset**

The dataset is stored in a CSV file named walkrun.csv, containing the following columns:

date: Date of data collection
time: Time of data collection
username: User who collected the data
wrist: Wrist where the device was placed (left or right)
activity: Activity type (0 for walking, 1 for running)
acceleration_x, acceleration_y, acceleration_z: Accelerometer readings along X, Y, and Z axes
gyro_x, gyro_y, gyro_z: Gyroscope readings along X, Y, and Z axes
Preprocessing

Missing Values: There are no missing values in the dataset.
Data Cleaning: Duplicates, if any, have been removed.
Feature Engineering: Additional features such as total acceleration magnitude and month of data collection have been extracted.
Data Transformation: Standardization has been applied to numerical features.
Train-Test Split: The dataset has been split into training and testing sets.
Models

Several classification models have been trained and evaluated on the dataset:

Logistic Regression
Support Vector Machine (SVM)
Decision Tree
Random Forest
The performance of each model is evaluated using accuracy score, confusion matrix, and classification report.

**Results**

The accuracy scores achieved by each model are as follows:

Logistic Regression: 95.89%
Support Vector Machine: 95.18%
Decision Tree: 99.57%
Random Forest: 99.83%
Based on the results, the Random Forest model demonstrates the highest accuracy in classifying walking and running activities.

**Requirements**

Python 3.x
Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

**Usage**

Clone the repository:
git clone <repository-url>
Navigate to the project directory:
cd walk-vs-run-classification
Install the required libraries:
pip install -r requirements.txt
Run the Jupyter Notebook walk_run_classification.ipynb to execute the code and explore the analysis
