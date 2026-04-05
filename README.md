# Titanic Survival Prediction using Machine Learning

## Project Overview

This project develops a machine learning classification model to predict whether a passenger survived the Titanic disaster. 
The model uses passenger attributes such as age, gender, ticket class, and other factors to make predictions.  

To ensure robust performance, the project incorporates cross-validation and hyperparameter tuning within a structured machine learning pipeline.

## Dataset
Dataset: Titanic Survival Dataset
Contains passenger information including: Age, Sex, Passenger class (Pclass), Fare, Embarked location.  

The dataset includes both numerical and categorical features, requiring preprocessing before model training.

## Data Preprocessing and Feature Engineering
- Handled missing values appropriately
- Separated numerical and categorical features
  
Applied:
- Standard Scaling for numerical data
- One-Hot Encoding for categorical data
- Integrated preprocessing steps into a pipeline for consistency
  
## Machine Learning Approach

A pipeline-based approach was used to streamline preprocessing and model training. This ensures that all transformations are consistently applied during both training and evaluation.  

## The workflow includes:

- Data preprocessing
- Feature transformation
- Model training
- Model evaluation
- Model Training and Evaluation
- Train-test split applied to evaluate generalisation performance
- Cross-validation performed to ensure robustness
- Hyperparameter tuning conducted using GridSearchCV to identify optimal model settings
- Model Comparison

## Two models were implemented and evaluated:

Random Forest Classifier : Used as the primary model due to its ability to capture complex patterns and handle feature interactions.  
Logistic Regression: Used as a simpler baseline model for comparison

Both models were trained using the same preprocessing pipeline and evaluation strategy to ensure a fair comparison.

## Results

The performance of both models was evaluated using standard classification metrics. 
All of the scores are slightly better for logistic regression than for random forest classification, although the differences are insignificant. 
Although the performances of the two models are virtually identical, the features that are important to the two models are very different. 
This suggests there must be more work to do to better grasp the actual feature importancdes. 
It's crucially important to realize that there is most likely plenty of dependence amongst these variables, and a more detailed modelling approach including correlation analysis is required to draw proper conclusions. 

Overall, Random Forest showed slightly better performance, making it the preferred model for this task.

## How to Run

- Clone the repository:

      git clone https://github.com/jsharonjr/Titanic-Survival-Prediction
  
- Navigate to the project folder:

      cd Titanic-Survival-Prediction
  
- Install dependencies:

      pip install numpy pandas scikit-learn matplotlib seaborn
  
- Open and run the notebook:
  - Open the .ipynb file in Jupyter or VS Code
  - Run all cells
 
## License
Distributed under the MIT License. See [LICENSE](https://github.com/jsharonjr/Titanic-Survival-Prediction?tab=MIT-1-ov-file) for more information.
