# PNEUMONIA-DETECTION-USING-DEEP-LEARNING-

![image](https://github.com/FridaOyucho/PNEUMONIA-DETECTION-USING-DEEP-LEARNING-/assets/63707906/c2389f52-a607-4680-8266-1547a50f82c6)



Authors: Jane Martha, Najma Abdi, Brian Ochieng, Eunice Ngunjiri, Jubilant Mutuku, Frida Oyucho

## Project Overview
The project focuses on leveraging a dataset of chest X-ray images to develop machine learning models capable of accurately diagnosing pneumonia. The dataset sourced from Kaggle, comprises of images classified into two categories: pneu,onia and normal. This project aims to build and optimize convolutional neural network(CNN) models to achieve high diagnostic accuracy.

## Business problem
![image](https://github.com/FridaOyucho/PNEUMONIA-DETECTION-USING-DEEP-LEARNING-/assets/63707906/43285e44-bee3-46a1-97fa-f120bad3c87b)



Early detection and treatment of pneumonia are essential for avoiding complications and enhancing clinical results.
Chest X-rays are a frequently used imaging modality for diagnosing pneumonia. Healthcare professionals, patients, hospitals,
researchers and government agencies stand to benefit from these advancements, using the advanced technology models to deepen disease understanding and ensure regulatory compliance.

## Data Understanding
Source: Kaggle's Chest X-Ray Images (Pneumonia) dataset. Structure: The dataset is organized into three primary directories: train: Contains training images categorized into 'PNEUMONIA' and 'NORMAL'. val: Contains validation images for model tuning and performance evaluation. test: Contains test images for final model evaluation.

## Objectives 
Traditionally, diagnosing pneumonia requires time-consuming physical examinations and lab tests,
often necessitating multiple doctor visits. We aim to develop a deep learning model capable of
accurately detecting pneumonia from chest x-ray images

## Methodology
Data modelling was based on clients tested for pneumonia with Xray test results as either normal or Pneumonia 
  1. Data preparation and understanding
  -   To understand the structure of the dataset first we examined the directory structure and counted the number of images in each class for training, validation, and testing sets.
  2. Exploratory Data analysis was done on: the training, validation and test datasets. This was done by:
    - visualizing outputs in Barcharts, to understand the distribution of data
    - Visualization of images to understand the dimensions and pixels values of images in order to perform preprocessing.
3. Data Preprocessing was done to prepare the data for modeling(Resizing the images and Normalization)

7. Data modelling was done using two models with hyperparameter tunings to improve their performances: 
  -  Baseline Convolutional Neural Network Model(CNN)
  -  Tuned Convolutional Neural Network Model(CNN)
  -  Complex Model
  -  ResNet50V2 Model

## Results
![image](https://github.com/FridaOyucho/PNEUMONIA-DETECTION-USING-DEEP-LEARNING-/assets/63707906/da71e7ff-6508-41ca-b29d-f00593233778)


We visualzed the data from the three datasets to check for class imbalance. From the barchart, the data was highly imbalanced.

Modelling:
![image](https://github.com/FridaOyucho/PNEUMONIA-DETECTION-USING-DEEP-LEARNING-/assets/63707906/398f5224-8eff-4763-9bc9-a0f812882ca7)


Duration:
  -  Baseline Model took 2hrs 42mins 18secs
  -  Tunned baseline model: 8hrs 44mins 19secs for the best trial
  -  Complex architecture: 2hrs 20mins 15sec
  -  ResNET59V2 model: 1hr 30mins

Model Comparison:
![image](https://github.com/FridaOyucho/PNEUMONIA-DETECTION-USING-DEEP-LEARNING-/assets/63707906/8c80708c-67d1-4268-bce3-2486d2d05fc9)


## Observations:
We observed that execution time decreases each time a new model is executed and the accuracy becomes better each time hence boosting performance.

The best model is the ResNET50V2, which has nalidation accuracy of 0.938 and took the shortest execution time of 1hr 30min 10 secs.

The least was Baseline model and the second improved model was complex architecutre.

Early Stoping model helped in minimizing overfitting hence boosting performance.

## Conclusion:
Incorperations of these models can help in boosting treatment, detecting level of pneumonia at different level in both first and critical stages and widening doctors knowledge in finding the best cure for pneumonia in both adults and children hence reducing death rates.

## Recommendation:

  1.  Validation the developed model through clinical trials is needed to ensure its reliability for diagnoses.
  2.  Focus on creating a system that functions effectively with limited computational resources
  3.  Further optimization of hyperparameters such as dropout rate and batch size to enhace model performance
  

