# Customer-Purchase-Prediction-Using-ANN

## Problem Statement
Businesses often need to identify customers who are likely to make a purchase so that marketing efforts can be targeted effectively. The objective of this project is to build an Artificial Neural Network (ANN) model that predicts whether a customer will make a purchase based on available customer features.

## Objective
Develop and evaluate an ANN-based binary classification model to predict customer purchase behavior and compare the performance of different optimizers.

## Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Seaborn

## Project Workflow
1. Data Loading and Exploration
2. Data Preprocessing
   - Handling missing values
   - Feature scaling
   - Train-test split
3. ANN Model Development
4. Model Training using Adam Optimizer
5. Model Training using SGD Optimizer
6. Model Evaluation
7. Performance Comparison
8. Results Interpretation

## ANN Architecture
- Input Layer: Number of neurons equal to input features
- Hidden Layer 1: Dense layer with ReLU activation
- Dropout: 0.3
- Hidden Layer 2: Dense layer with ReLU activation
- Dropout: 0.2
- Output Layer: 1 neuron with Sigmoid activation

## Model Performance

| Adam | Optimizer |
|:-----:|:---------|
| Metric | Score |
| Accuracy | 0.75 |
| Precision |	1.00 |
| Recall | 0.375 |
| F1 Score | 0.545 |

## SGD Optimizer
| Metric | Score |
|:------:|:-----:|
| Accuracy | 0.75 |
| Precision |	1.00 |
| Recall | 0.375 |
| F1 Score | 0.545 |

### Best Optimizer
Although both optimizers achieved identical performance metrics, SGD converged in only 4 epochs compared to 50 epochs for Adam, making SGD more efficient for this dataset.

## Confusion Matrix
| Actual / Predicted | 0 | 1 |
|------|------|-----|
| 0 | 12 | 0 |
| 1 |	5 |	3 |

## Key Insights
- The model achieved 75% classification accuracy.
- Precision of 100% indicates that every predicted purchaser was actually a purchaser.
- Recall of 37.5% indicates that several actual purchasers were missed.
- SGD converged significantly faster than Adam while maintaining the same performance.
- Dropout layers helped reduce overfitting and improve model generalization.

## Business Recommendations
- Use the model to identify high-confidence potential buyers for targeted marketing campaigns.
- Improve recall by collecting more balanced data or applying class imbalance techniques such as SMOTE.
- Continuously monitor model performance and retrain periodically as customer behavior changes.
- Experiment with additional features and hyperparameter tuning to improve prediction performance.

## Skills Demonstrated
- Data Preprocessing
- Feature Scaling
- Artificial Neural Networks (ANN)
- Binary Classification
- Deep Learning
- TensorFlow/Keras
- Model Evaluation
- Hyperparameter Tuning
- Confusion Matrix Analysis
- Python Programming
