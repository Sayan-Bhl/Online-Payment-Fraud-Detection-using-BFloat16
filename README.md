# Online Payment Fraud Detection using BFloat16 Dtype

This project aims to demonstrate the benefits of using the BFloat16 data type for training machine learning models in the context of online payment fraud detection. By utilizing BFloat16, we can significantly reduce the training time without compromising the model's performance.

## Table of Contents

- [Introduction](#introduction)
- [Usage](#usage)
- [Dataset](#dataset)
- [Steps](#steps)
- [Results](#results)
- [BFloat16 Data Type](#bfloat16-data-type)


## Introduction

Online payment fraud is a significant concern for e-commerce platforms and financial institutions. Detecting fraudulent transactions accurately and efficiently is crucial to protect both merchants and consumers. This project focuses on building a machine learning model using BFloat16 data type to accelerate the training process while maintaining high detection accuracy.
<a name='usage'></a>
## Usage

To run this project locally, please follow these steps:

1. Right click on 'Open in Colab'
2. Go to File->Save a copy on Drive
3. Click on 'Open in new Tab'
4. Add .csv file to Drive
5. Click on Runtime->Run all in Colab

## Dataset

The dataset used in this project contains a collection of online payment transactions, including both legitimate and fraudulent transactions. The dataset is available at [https://www.kaggle.com/datasets/jainilcoder/online-payment-fraud-detection] and is provided in a CSV format. Make sure to download the dataset and place it in the Drive before running the project.

## Steps

1. Data Collection

2. Data Visualization

3. Data Preprocessing
   - OneHotEncoding for encoding object type data
   - SMOTE for oversampling
    
4. Train The Model
   - RandomForestClassifier
5. Evaluate The Model

## Results

The use of BFloat16 data type in this project significantly reduces the training time for machine learning models while maintaining high accuracy in detecting online payment fraud. The results obtained from this project demonstrate the efficacy of using BFloat16 to expedite the training process.

| Model                  | Training Time (BFloat16) | Training Time (Float32) |
|------------------------|--------------------------|-------------------------|
| RandomForestClassifier | 1min 58s                 | 3min 54s                |



| Model                  | Accuracy (BFloat16)      | Accuracy (Float32) |
|------------------------|--------------------------|-------------------------|
| RandomForestClassifier | 0.9992715265095197       | 0.9993021742615463      |


Note: The above tables show the training times and accuracy achieved by Random Forest Classifier model using BFloat16 and Float32 data types. The results highlight the reduced training time when using BFloat16 without significant impact on accuracy.

## BFloat16 Data Type

The BFloat16 data type is a floating-point format that provides a compromise between the memory footprint of 16-bit floating-point numbers and the precision of 32-bit floating-point numbers. It uses 8 bits for the exponent and 7 bits for the significand, resulting in a range of values that can be represented with reduced precision compared to Float32.

By using BFloat16, we can take advantage of its smaller memory footprint and the ability to perform calculations faster compared to Float32. This reduction in precision can be acceptable in certain applications, such as machine learning, where the emphasis is often on the overall trends and patterns rather than exact numerical values.

In this project, we leverage the benefits of BFloat16 to train machine learning models for online payment fraud detection. By using this data type, we can achieve significant speedup in the training process while maintaining the necessary accuracy for effective fraud detection.


