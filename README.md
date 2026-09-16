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
## SHAP Explanation

SHAP was used to understand how individual features contributed to the model's prediction.

For the analyzed Standing sample, SHAP identified the features that had the strongest influence on the prediction.
## LIME Explanation

LIME was used to explain the same Standing prediction by creating small variations of the input sample and observing how the model's prediction changed.

The explanation showed which features supported or moved away from the Standing prediction.
## SHAP vs LIME Comparison

For the analyzed Standing sample, SHAP and LIME identified three common important features:

- tBodyGyroJerk-arCoeff()-X,2
- tBodyGyroJerk-entropy()-Y
- tBodyGyroJerk-arCoeff()-Y,1

Both methods also agreed on the direction of influence for these features.
## Results

The Deep Learning model achieved approximately 93% accuracy on the test set.

The SHAP and LIME explanations showed agreement for the analyzed Standing sample, with three common important features identified by both methods.
## Technologies Used

- Python
- TensorFlow / Keras
- SHAP
- LIME
- Pandas
- NumPy
- Matplotlib
- Google Colab
## Limitations

The SHAP and LIME comparison was performed on one Standing sample. Therefore, the observed agreement cannot be generalized to all samples or activities.

A larger multi-sample analysis could be performed as future work.
## Future Work

- Analyze SHAP and LIME explanations across multiple samples.
- Compare the consistency of important features across samples.
- Investigate explanations for different human activities.
