 
# Interpretability of Machine Learning Algorithms for Alzheimer's Disease Prediction via-SHAP method

## Project Overview

This project delves into the interpretability of machine learning algorithms, particularly focusing on the SHAP (SHapley Additive exPlanations) technique. The objective is to gain insights into how different features contribute to the prediction of Alzheimer's disease.

## Dataset

The project utilizes the OASIS longitudinal dataset, which contains clinical and demographic information about individuals with and without Alzheimer's disease. The dataset is preprocessed to handle missing values and encode categorical features.

## Machine Learning Algorithms

Three machine learning algorithms are employed for prediction:

- **Decision Tree (DT)**: A simple tree-based model.
- **Random Forest (RF)**: An ensemble method that combines multiple decision trees.
- **XGBoost (XGB)**: A gradient boosting algorithm known for its high performance.

## SHAP Interpretation

The SHAP (SHapley Additive exPlanations) library is used to interpret the predictions made by these algorithms. SHAP provides both local and global explanations:

- **Local Explanations:** Focus on individual data points, showing how each feature contributes to the specific prediction for that point.
- **Global Explanations:** Provide an overall view of feature importance across the entire dataset.

## Analysis and Results

The analysis reveals the following key findings:

- **M/F (Male/Female):** This feature is consistently identified as the most influential factor, with a substantial impact on the predicted probability of Alzheimer's disease. Being male significantly increases the likelihood of developing the disease.
- **Education Level (EDUC):** Higher education levels are generally associated with a lower probability of Alzheimer's disease.
- **Socioeconomic Status (SES) and Age:** These features have less pronounced effects compared to M/F and EDUC.
- **Local vs. Global Explanations:** SHAP's local explanations provide valuable insights into individual cases, while global explanations reveal the overall feature importance in the model.

## Conclusion

This project demonstrates the effectiveness of SHAP for interpreting machine learning models in the context of Alzheimer's disease prediction. The findings highlight the importance of gender and education level as key factors in the disease's development.

## Usage

1. Clone this repository.
2. Upload the 'oasis_longitudinal.csv' dataset to Colab.
3. Run the notebook provided to train the models and generate SHAP explanations.

## Dependencies

- Python 3
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- TensorFlow
- SHAP

## Contributing

Contributions are welcome! Please open an issue or pull request to suggest improvements or add new features.

## License

This project is licensed under the MIT License.
