SVM on Iris Dataset
Overview
This project applies a Support Vector Machine (SVM) classifier to the Iris dataset to predict flower species based on four numerical features.

Steps
Load the Iris dataset using seaborn

Perform EDA (pairplot + KDE for Setosa)

Split data into training and testing sets

Train an SVC model

Evaluate using confusion matrix and classification report

Tune hyperparameters using GridSearchCV

Results
Base SVM accuracy: 98%

GridSearchCV produced the same accuracy

The dataset is simple, so SVM performs extremely well

Requirements
numpy
pandas
seaborn
matplotlib
scikit-learn
