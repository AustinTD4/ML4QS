# Machine Learning for the Quantified Self: Activity Recognition & Cadence Prediction

This repository contains code, data, and a report for a school project focused on recognizing user activities (sitting, walking, running, and cycling) and predicting current cadence (steps per min or revolutions per min) based on a ten-second window of accelerometer and gyroscope data.

## Project Overview

- **Duration**: 4 weeks
- **Collaboration**: This project was a joint effort between a Austin Dickerson and Georgios Xanthopolous. They gathered data from cellphones by conducting a series of movement experiments, resulting in a few hours of data. They manually labeled this data to create a supervised learning environment. Austin focused on Machine Learning and Feature Engineering, while Georgios Focused on data analysis.
- **Origins**: This project's goal was devised by the group members, and supervised by a postgrad advisor. All code in this repository represent Austin Dickerson's original work, however raw data and the report were both a collaboration between Austin and Georgios.

## Data Processing & Feature Engineering

Principal Component Analysis (PCA) was employed to reduce the data's complexity from its original 9 inputs. Additionally, the Kalman filter and Fourier transformations were used for data filtering and transformation. Statistical metrics were integrated into the raw data to provide distribution insights.

The different machine learning models explored both **dense** and **sparse** data representations:
- **Dense Representation**: Maintained all available features, presenting a comprehensive view of the data.
- **Sparse Representation**: Focused on the most significant features, discarding redundant or less informative ones.

## Machine Learning Models

Deep Neural Networks, LSTMs, TCNs, and Random Forests were applied for two main tasks:
- **Classification**: Recognizing the user's activity.
- **Regression**: Predicting the current cadence.

Detailed results and insights are elaborated in the report ([ML4QS_Report](#)) included in this repository.

### FILES:
- **10 Second Sample Windows and Fourier.ipynb**: This notebook processes raw data into 10-second windows and applies Fourier transformations to extract frequency domain features.
- **Creating Dataset Week 1.ipynb**: An initial notebook documenting the steps and methods used to create our dataset during the first week of the project.
- **Making Samples and Neural Networks.ipynb**: This notebook outlines the procedure for segmenting the data into samples and the subsequent development and testing of Neural Network models.
- **TCN_LSTM.ipynb**: Dedicated to the design, implementation, and evaluation of Temporal Convolutional Networks (TCN) and Long Short-Term Memory (LSTM) models for our dataset.

### FOLDERS:
- **Data Samples**: Contains true original data gathered from experimenters measured at 20Hz.
- **Filtered Data**: Contains original and PCA transformed data after using the Kalman filter to remove noise and outliers.
- **Final Data**: Contains the data used to train the machine learning algorithms.
- **Fourier**: Contains visualizations for the Fourier transformations of each input from each activity sample.
- **Grid_Search_Tuning**: Contains the code to perform hyperparameter tuning for the deep neural network classification and regression models

## Results
- **ML4QS Report**: Contains detailed results of the experiment and performance improvements over the benchmark
