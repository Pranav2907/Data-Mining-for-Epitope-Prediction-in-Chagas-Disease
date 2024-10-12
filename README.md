# Data Mining Project - Predictive Analysis & Insights Extraction

This repository contains the code and methodologies used in a data mining project for the MSc in Artificial Intelligence program. The project focuses on deriving actionable insights and creating predictive models through various data mining and machine learning techniques.

## Project Overview

The project involved analyzing a dataset with substantial class imbalance to predict outcomes on a holdout set. Key stages included Exploratory Data Analysis (EDA), feature reduction, data preprocessing, model selection, and hyperparameter tuning. The Gradient Boosting Classifier, selected for its high F1, accuracy, and balanced accuracy scores, serves as the final model in a robust data pipeline.

## Repository Structure

- **data/**: Raw and preprocessed datasets (initial data not included).
- **notebooks/**: Jupyter notebooks detailing each step, including EDA, feature selection, and model training.
- **scripts/**: Python scripts for data preprocessing, feature reduction, model training, and evaluation.
- **models/**: Saved models used for prediction.
- **results/**: Final predictions on the holdout dataset and model evaluation metrics.

## Methodology

1. **EDA and Data Preprocessing**:
   - **Scaling**: Applied MinMaxScaler to normalize the data.
   - **Outliers**: Used ECOD for outlier detection and Winsorization for handling extreme values.
   - **Missing Values**: Dropped features with high missing data and used median imputation for the rest.

2. **Feature Reduction**:
   - Implemented Variance Threshold, Information Gain, and MRMR to select top features, refining down to the most predictive 30 features.

3. **Class Imbalance Handling**:
   - Applied various sampling techniques, with ASADYN showing the best performance with Decision Tree Classifier, resulting in balanced accuracy and F1 improvements.

4. **Modeling**:
   - Explored Logistic Regression, RandomForest, and Decision Tree classifiers, with Gradient Boosting Classifier emerging as the optimal choice.

5. **Pipeline**:
   - Custom pipeline integrating data preprocessing, feature selection, and final model was created for efficient predictions on new data.

## Results

The Gradient Boosting Classifier achieved an F1 Score of 0.77, with an accuracy of 0.73, making it the most effective model for this dataset. Predictions on the holdout set are saved as a CSV file.

## Conclusions & Future Directions

The project successfully identified significant predictors and provided actionable insights. Future work may explore adding data sources and using advanced ML techniques like deep learning for enhanced performance.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Pranav2907/Data-Mining-for-Epitope-Prediction-in-Chagas-Disease.git
