# Laptop Price Prediction using specifications 💻
## Overview
This project is part of the final assignment of IronHack Data Analytics bootcamp, for the Data Science track. The objective is to predict the 
Laptop Price Prediction using specifications using various machine learning regression and to evaluate their performance. Given the trend of new technologies
the focus on the models would be identifying the prices by their specs.

## Dataset
The dataset used for this project they were titled laptops_test.csv and laptops_train.csv and it is sourced from Kaggle. It contains various features related to computer hardware and sodftware.

 ### Features
 
 ### Training Dataset (laptops_train.csv)

    Entries: 977
    Columns: 13
    Features:
        Manufacturer: Brand of the laptop (e.g., HP, Asus, Dell)
        Model Name: Model designation of the laptop
        Category: Type of laptop (e.g., Notebook, Gaming, 2 in 1 Convertible)
        Screen Size: Size of the screen (e.g., 15.6")
        Screen: Screen specifications including resolution and type (e.g., Full HD 1920x1080)
        CPU: Processor details (e.g., Intel Core i7 7500U 2.7GHz)
        RAM: Size of the RAM (e.g., 8GB)
        Storage: Storage capacity and type (e.g., 256GB SSD)
        GPU: Graphics processing unit details (e.g., Nvidia GeForce GTX 1050)
        Operating System: Operating system (e.g., Windows)
        Operating System Version: Version of the operating system
        Weight: Weight of the laptop (e.g., 2.5kg)
        Price: Price of the laptop (in float)

 ### Testing Dataset (laptops_test.csv)

    Entries: 325
    Columns: 13
    Features: Same as the training dataset, except the Price column is used for predictions and is not present in the testing dataset for evaluation purposes.
