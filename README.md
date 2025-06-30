# AI-ML-task-5
# Heart Disease Prediction using Decision Tree and Random Forest

This project involves training and evaluating Decision Tree and Random Forest classifiers on the Heart Disease dataset from Kaggle. It focuses on tree visualization, overfitting analysis, feature importance interpretation, and model evaluation using cross-validation.

## Dataset

- Source: [Kaggle - Heart Disease UCI Dataset](https://www.kaggle.com/ronitf/heart-disease-uci)
- Format: CSV (`heart.csv`)
- Target Column: `target` (1 = Disease, 0 = No Disease)

##  Tasks Performed

1. **Train a Decision Tree Classifier**
   - Visualized the decision tree using `plot_tree`.

2. **Overfitting Analysis**
   - Compared full tree vs. depth-limited tree.
   - Controlled tree depth using `max_depth` parameter.

3. **Train a Random Forest Classifier**
   - Used 100 estimators for better generalization.
   - Compared accuracy with Decision Tree.

4. **Feature Importance**
   - Interpreted top contributing features using `feature_importances_`.

5. **Cross-Validation**
   - Evaluated model stability using 5-fold `cross_val_score`.

## Model Performance

| Model           | Train Accuracy | Test Accuracy | CV Mean Accuracy |
|----------------|----------------|----------------|------------------|
| Decision Tree  | 100%            | ~98.5%         | —                |
| Random Forest  | 100%            | ~98.5%         | ~99.71%          |

##  Feature Importance Example
| Feature         | Importance |
| --------------- | ---------- |
| cp (chest pain) | 0.15       |
| thalach         | 0.14       |
| oldpeak         | 0.13       |
| ca              | 0.12       |
| ...             |            |

## Requirements

```bash
pandas
numpy
scikit-learn
matplotlib
seaborn

## Install using:
pip install pandas numpy scikit-learn matplotlib seaborn
## Project Structure
├── heart.csv                  # Dataset
├── heart_disease_model.ipynb # Colab notebook
├── README.md                 # This file

 ##How to Run
1) Upload heart.csv in Colab.
2) Run the notebook cells step-by-step.
3) Visualize the decision tree, evaluate accuracy, and plot feature importanc

