
# Predicting Gas Production in Wells Using Linear Regression

This project explores the development and evaluation of linear regression models to predict gas production in wells for **Gaz-Taz-Vaz-Neft**. The analysis is documented in a single Jupyter Notebook, with accompanying data provided in the `data` folder.

## Project Overview

The primary goal of this project is to build robust and accurate regression models for predicting gas production. The workflow includes:
- **Data analysis and preprocessing**: Analyzing the dataset to identify and exclude irrelevant or highly correlated features.
- **Linear regression modeling**: Building baseline models and comparing their performance.
- **Polynomial feature generation**: Capturing complex relationships in the data using third-order polynomial features.
- **Regularization**: Applying Lasso, Ridge, and ElasticNet regression to improve generalization and reduce overfitting.

## Results

| Model Name          | Hyperparameters           | Polynomial Features | MAE on Training Folds | MAE on Validation Folds | MSE on Training Folds | MSE on Validation Folds |
|---------------------|---------------------------|----------------------|------------------------|-------------------------|------------------------|-------------------------|
| Linear Regression   |                           | True                 | 484.69                | 571.73                 | 379,123.16            | 528,466.46             |
| Lasso               | alpha=24.42               | True                 | 495.75                | 556.72                 | 400,220.99            | 512,196.10             |
| Ridge               | alpha=3.73                | True                 | 484.28                | 567.64                 | 384,697.02            | 538,915.26             |
| ElasticNet          | alpha=24.42, l1_ratio=1.0 | True                 | 495.75                | 556.72                 | 400,220.99            | 512,196.10             |

## Key Findings

1. **Best Models**:
   - The **Lasso** and **ElasticNet** models demonstrated the best performance on validation folds, achieving the lowest MAE and MSE metrics.

2. **Regularization Benefits**:
   - Regularization techniques significantly improved the generalization ability of the models, with ElasticNet combining L1 and L2 regularization for robust performance.

3. **Impact of Polynomial Features**:
   - Polynomial features helped capture complex relationships in the data, but their use increased the risk of overfitting without proper regularization.

## Files in the Project

- `notebook.ipynb`: Jupyter Notebook containing all the analysis, modeling, and results.
- `data/unconv.csv`: Dataset used for the analysis.
- `README.md`: Project documentation.

## How to Run the Notebook

1. Clone or download the project folder.
2. Ensure that the `unconv.csv` file is in the `data` folder.
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook notebook.ipynb
   ```
4. Follow the steps in the notebook to replicate the analysis and results.

## Technologies Used

- **Python**: Core programming language for the project.
- **pandas, NumPy**: Libraries for data manipulation and numerical computations.
- **scikit-learn**: Used for model building, evaluation, and regularization.
- **matplotlib, seaborn**: Libraries for data visualization.

## Conclusion

This project demonstrates the effective use of linear regression models, polynomial feature engineering, and regularization to predict gas production with high accuracy. The **Lasso** and **ElasticNet** models are recommended for deployment due to their balance of precision and generalization.

---

Feel free to explore the notebook and data, and share feedback to enhance this analysis!
