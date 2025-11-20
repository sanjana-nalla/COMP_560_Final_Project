Depression Prediction Using Machine Learning

COMP 560 Final Project — Harjas Kaur, Sanjana Nalla, Nidhi Padala, Tejaswi Paladugu

This project explores how different machine learning models perform when predicting depression using a large synthetic mental health survey dataset from the Kaggle Playground Series (Season 4, Episode 11). Each entry in the dataset represents a generated survey response with demographic, academic, lifestyle, and stress-related features, paired with a binary depression label. Our goal was to evaluate how well various models could classify respondents as depressed or non-depressed.

Project Overview

We compared four approaches of increasing complexity:

Gaussian Naive Bayes – a simple probabilistic baseline

Logistic Regression – a linear, interpretable model using detailed one-hot encoded features

PCA-Based Classifier – a 2D projection for visualizing and modeling structure

Feedforward Neural Network – a non-linear model capturing more complex interactions

Key Results

Logistic Regression significantly outperformed Naive Bayes, showing the value of richer feature encoding.

PCA (2 components) performed unexpectedly well, achieving ~0.99 accuracy and ~0.999 ROC AUC on both CV and validation sets.

Neural Network achieved ~0.94 accuracy with strong probability separation, offering useful confidence insights even though its accuracy was slightly lower.

Across models, depression labels were predicted with high accuracy, suggesting strong linear structure in the dataset.

Limitations

The dataset is synthetic and may not fully represent real clinical responses. Results may differ on real-world mental health data.

Future Work

Potential next steps include applying the pipeline to real screening surveys, experimenting with deeper architectures, and analyzing feature importance.
