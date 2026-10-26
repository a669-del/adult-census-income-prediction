# Adult Census Income Prediction

## Project Overview
This project uses machine learning to predict whether an individual earns more than $50,000 per year based on census and employment-related attributes.

## Objectives
- Explore and analyze census data.
- Perform data preprocessing and feature engineering.
- Train classification models.
- Evaluate model performance.

## Technologies Used
- Python
- Google Colab
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn

## Project File
- `Adult_Census_Income_Prediction.ipynb` — Jupyter notebook containing the project code and analysis.

## How to Run
1. Open the notebook in Google Colab.
2. Upload or load the required dataset.
3. Run the notebook cells in order.

## Disclaimer
The predictions are estimates based on the dataset and should not be used as the sole basis for decisions about individuals.
## Machine Learning Models

The project implements and evaluates three classification algorithms:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

## Model Performance

The models were evaluated on a test set of 6,508 records.

| Model | Accuracy |
|---|---:|
| Logistic Regression | 85.79% |
| Decision Tree | 86.46% |
| Random Forest | 86.85% |

Random Forest achieved the highest accuracy among the three models in this experiment.

## Evaluation Metrics

The project uses accuracy, precision, recall, F1-score, and confusion matrices to evaluate model performance.

For the Random Forest model, the classification report shows:
- **Accuracy:** 86.85%
- **Precision for income above $50K:** 0.80
- **Recall for income above $50K:** 0.60
- **F1-score for income above $50K:** 0.69

These results indicate that the model performs better at identifying the `<=50K` income class than the `>50K` class. The results should be interpreted with this class-wise difference in mind.

## Feature Importance

The Random Forest feature-importance analysis identifies capital gain, marital status, education level, age, and relationship status among the influential features in the trained model.

## Saved Model Files

The notebook saves the following files:
- `random_forest_model.pkl`
- `preprocessor.pkl`
- `label_encoder.pkl`

These files support reuse of the trained model and its preprocessing components.
