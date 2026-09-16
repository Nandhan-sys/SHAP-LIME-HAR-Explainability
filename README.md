# Comparing SHAP and LIME for Explaining Deep Learning Predictions
## Project Overview

This project compares SHAP and LIME for explaining predictions made by a Deep Learning model trained on the UCI Human Activity Recognition (HAR) dataset.

## Dataset

The UCI Human Activity Recognition (HAR) dataset contains sensor data collected from smartphones while people performed different physical activities.

- 7,352 training samples
- 2,947 testing samples
- 561 features
- 6 activities
## Deep Learning Model

A fully connected neural network was used to classify the six human activities.

Architecture:

561 features → 128 → 64 → 32 → 6 outputs

The model was trained using the Adam optimizer and categorical cross-entropy loss.
