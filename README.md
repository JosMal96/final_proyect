# Laptop Price Prediction using specifications 💻
## Overview
This project is part of the final assignment of IronHack Data Analytics bootcamp, for the Data Science track. The objective is to predict the 
Laptop Price Prediction using specifications using various machine learning regression and to evaluate their performance. Given the trend of new technologies
the focus on the models would be identifying the prices by their specs.

## Dataset
The dataset used for this project they were titled laptops_test.csv and laptops_train.csv and it is sourced from Kaggle. It contains various features related to computer hardware and sodftware.

Sure, here's a summary for your README file on GitHub:

---

## Laptops Dataset

### Overview

This repository contains datasets of laptops with various features. The data is divided into two files: a training dataset (`laptops_train.csv`) and a testing dataset (`laptops_test.csv`). These datasets can be used for tasks such as price prediction, classification, and other machine learning projects. I've used to prediction on the price.

### Datasets

#### Training Dataset (`laptops_train.csv`)

- **Entries**: 977
- **Columns**: 13
- **Features**:
  1. **Manufacturer**: Brand of the laptop (e.g., HP, Asus, Dell)
  2. **Model Name**: Model designation of the laptop
  3. **Category**: Type of laptop (e.g., Notebook, Gaming, 2 in 1 Convertible)
  4. **Screen Size**: Size of the screen (e.g., 15.6")
  5. **Screen**: Screen specifications including resolution and type (e.g., Full HD 1920x1080)
  6. **CPU**: Processor details (e.g., Intel Core i7 7500U 2.7GHz)
  7. **RAM**: Size of the RAM (e.g., 8GB)
  8. **Storage**: Storage capacity and type (e.g., 256GB SSD)
  9. **GPU**: Graphics processing unit details (e.g., Nvidia GeForce GTX 1050)
  10. **Operating System**: Operating system (e.g., Windows)
  11. **Operating System Version**: Version of the operating system
  12. **Weight**: Weight of the laptop (e.g., 2.5kg)
  13. **Price**: Price of the laptop (in float)

#### Testing Dataset (`laptops_test.csv`)

- **Entries**: 325
- **Columns**: 13
- **Features**: Same as the training dataset, except the `Price` column is used for predictions and is not present in the testing dataset for evaluation purposes.

## Methodology

### 1. Data Collection

The datasets were gathered to provide extensive information on laptops, including specifications such as manufacturer, model name, category, screen size, resolution, CPU, RAM, storage, GPU, operating system, weight, and price. These features are essential for analyzing laptop configurations and market pricing.

### 2. Data Preprocessing

**Loading the Data**:
- The datasets are loaded into pandas DataFrames for efficient data manipulation and analysis.

**Data Cleaning**:
- Handle missing values, particularly in the `Operating System Version` column.
- Ensure data types are consistent, converting strings to appropriate numeric types where necessary (e.g., weight, RAM and storage).

### 3. Exploratory Data Analysis (EDA)

**Descriptive Statistics**:
- Calculate summary statistics for numerical features (e.g., mean, median, standard deviation).
- Analyze frequency distribution for categorical features.

## Methodology

### 1. Data Collection

The datasets were collected to provide comprehensive information about laptops, encompassing various features like manufacturer, model name, category, screen size, screen specifications, CPU, RAM, storage, GPU, operating system, weight, and price. These datasets form the basis for analyzing laptop configurations and market pricing.

### 2. Data Preparation

**Loading the Data**:
- The datasets (`laptops_train.csv` and `laptops_test.csv`) are loaded into pandas DataFrames for efficient data manipulation and analysis.

**Data Cleaning**:
- Handle missing values, especially in the `Operating System Version` column.
- Convert data types where necessary, such as transforming weight from string to numeric values.

### 3. Exploratory Data Analysis (EDA)

**Descriptive Statistics**:
- Calculate summary statistics for numerical features like price and weight.
- Analyze the frequency distribution of categorical features like manufacturer, category, and operating system.

### 4. Feature Engineering and Preparation

- We defined the features and defined the target variables.
- Process the data and we do the numeric colums and categorical colums.
- Numeric Colums: Weight, RAM, Storage.
- Categorical columns where the other ones as CPU, GPU and etc.
- We did put the: Hot encoder, impute the data.
- We do the processor as the final step.

### 6. Model Building

**Model Selection**:
- Experiment with different machine learning algorithms such as Linear Regression, Decision Trees, Random Forest, and Gradient Boosting to find the best fit for the data.

**Model Training**:
- Train the models on the training dataset and fine-tune hyperparameters using techniques like cross-validation.

**Model Evaluation**:
- Evaluate the models using the validation set with performance metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²).
- Compare model performances and select the best-performing one.

## 7. Model Testing

### Results

#### K-Nearest Neighbors

 - **Mean Squared Error**: 5092063222672.665
 - **Mean Absolute Error**: 1375112.0317707267
 - **R^2 Score**:  0.871

#### Lineal Regression

 - **Mean Squared Error**: 3041503683489.974
 - **Mean Absolute Error**: 1203118.3826481747
 - **R^2 Score**:  0.923
   
#### Random Forest

 - **Mean Squared Error**: 1007089420347.268
 - **Mean Absolute Error**: 631486.2035689193
 - **R^2 Score**:  0.974

#### Gradient Boosting

 - **Mean Squared Error**: 4040249972207.7935
 - **Mean Absolute Error**: 1535678.5313377182
 - **R^2 Score**: 0.898

## 7. Imported pickle into the dataset
- We saved the best model from the dataset  and the we imported the pickle into the test dataset to predic the model.

## 8. The results of random forest
- The results we got from our best model imported into the test dataset was 0.76% which is not bad at all.

## 7. Conclusions
- The performance on the test data was lower with an R^2 score of 0.7589, suggesting that the model might be overfitting the training data or the test data might have different characteristics.


## Presentation

You can view the detailed presentation for this project [Laptop Price Prediction using specifications](https://www.canva.com/design/DAGJXlgohvs/EsFEXIt6WOFEjZTKsXpkwQ/edit).

