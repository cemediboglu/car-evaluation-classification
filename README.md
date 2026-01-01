Maker: Mehmet Cem Ediboglu
# Car Evaluation - Decision Tree Optimization

This project focuses on predicting the acceptability of cars based on their technical characteristics. I implemented a **Decision Tree Classifier** and performed rigorous **Hyperparameter Tuning** using **GridSearchCV** to achieve the highest predictive performance.

##  Project Highlights
- **Exploratory Data Analysis (EDA):** Cleaned and transformed raw categorical data.
- **Advanced Preprocessing:** Utilized `OrdinalEncoder` to preserve hiyerarchy in features and `ColumnTransformer` for a streamlined pipeline.
- **Hyperparameter Optimization:** Conducted a comprehensive grid search over `max_depth`, `criterion`, and `splitter` to prevent overfitting and underfitting.
- **Performance Evaluation:** Analyzed models using Confusion Matrices and Classification Reports to handle class imbalances.

## Tech Stack
- **Python**
- **Scikit-learn** (Model building & Validation)
- **Pandas & NumPy** (Data Manipulation)
- **Matplotlib & Seaborn** (Visualization of the Decision Tree)

## Dataset Information
The dataset consists of 1728 instances with 6 features:
- **Buying Price** (vhigh, high, med, low)
- **Maintenance Cost** (vhigh, high, med, low)
- **Number of Doors** (2, 3, 4, 5-more)
- **Capacity** (2, 4, more persons)
- **Luggage Boot Size** (small, med, big)
- **Safety Rating** (low, med, high)
- **Target:** Class (unacc, acc, good, vgood)

## Key Results
- **Initial Baseline:** Started with a shallow tree (`max_depth=3`) which resulted in poor recall for minority classes.
- **Optimized Model:** After `GridSearchCV` with 5-fold cross-validation, the model's accuracy and confusion matrix improved significantly.
- **Feature Importance:** Discovered that `persons` (capacity) and `safety` are the most critical factors in car evaluation.

## Repository Structure
- `car-evaluation-decision-tree-optimization.ipynb`: Full Python implementation and analysis.
- `README.md`: Project documentation.

---
*Developed as part of my Data Science Portfolio.
