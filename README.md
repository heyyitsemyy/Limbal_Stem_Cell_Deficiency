# Limbal_Stem_Cell_Deficiency

Goal/Objective: Create machine learning models to identify the best location to count stem cells and nerves in individuals with limbal stem cell deficiency based on microscopy images of the eye. The cell count and nerve count will assist clinicians in determining the severity of the disease

Information:

  ML Model: logistic regression
  Evaluation Metric: mean absolute error
  Data Preparation: Created masks and used the Pyradiomics Python Library to extract features from each image (radiomics_features function). Appended labels and normalized each column of the feature matrix.
  Results: 
    Cell Model: 5.533
    Nerve Model: 6.533
 
 
 Functions:

radiomics_features: creates a feature matrix for training
mean_norm: normalizes each columns in a data frame
logreg_classifier: initializes and trains a logistic regression model
photo_chooser: outputs a list of images above a 85% threshold to be used in the next step of the pipeline
Evaluation: evaluates the logistic regression model
logreg_classifier_features: initializes and trains a logistic regression model w/ given feature matrix

