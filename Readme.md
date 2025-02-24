## Evaluation of Regression & Classification Models

Author: [Hamza Kamelen](https://www.linkedin.com/in/hamzakamelen)
### Introduction

The primary goal of this notebook is to evaluate the performance of regression and classification models, both regression and classification models is used to identify the accurate model for prediction the target variable. This notebook is divided into two parts, the first part is for regression models and the second part is for classification models. The dataset used in this notebook is the `Diamond Dataset` which is available in the `seaborn` library. The target variable for regression is `price` and for classification is `cut`. 

This dataset contain 10 columns and 53940 rows but for simplicity, only 10000 rows are used in this notebook. 

### Goals
- To select the best model for regression and classification
- To evaluate the performance of the models
- To compare the performance of the models

### Evaluated Algorithms:

**Regression Models:**
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor
- K-Nearest Neighbors Regressor
- XGBoost Regressor
- LightGBM Regressor
- CatBoost Regressor
- AdaBoost Regressor

**Classification Models:**
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- Support Vector Classifier
- K-Nearest Neighbors Classifier
- XGBoost Classifier
- LightGBM Classifier
- CatBoost Classifier
- AdaBoost Classifier

### Dataset Description:

The dataset contains the following columns:

- `carat`: weight of the diamond (0.2--5.01)
- `cut`: quality of the cut (Fair, Good, Very Good, Premium, Ideal)
- `color`: diamond colour, from J (worst) to D (best)
- `clarity`: a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
- `depth`: total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
- `table`: width of top of diamond relative to widest point (43--95)
- `price`: price in US dollars (\$326--\$18,823)
- `x`: length in mm (0--10.74)
- `y`: width in mm (0--58.9)
- `z`: depth in mm (0--31.8)


### Conclusion of Regression Models:
- The best model for regression is `LightGBM Regressor` with an `R2 Score` of `0.978657` and `RMSE` of `586.5` and `MAE` of `309.499`.
- The 2nd best model for regression is `CatBoost Regressor` with an `R2 Score` of `0.978375` and `RMSE` of `590.413` and `MAE` of `310.54`.
- The worst model for regression is `SVR` with an `R2 Score` of `0.725292` and `RMSE` of `2104.308299` and `MAE` of `1055.015279`.


### Conclusion of Classification Models:

- The best model for classification is `LightGBM Classifier` with an `Accuracy` of `0.7740` and `F1 Score` of `0.768098`.
- The 2nd best model for classification is `Gradient Boosting Classifier` with an `Accuracy` of `0.7710` and `F1 Score` of `0.764266`.
- The worst model for classification is `K-Nearest Neighbors Classifier` with an `Accuracy` of `0.6245` and `F1 Score` of `0.595863`.

---

### Conclusion of Evaluation:
- The best model for Regression is `LightGBM Regressor` with an `R2 Score` of `0.978657` and `RMSE` of `586.5` and `MAE` of `309.499`.
- The best model for Classification is `LightGBM Classifier` with an `Accuracy` of `0.7740` and `F1 Score` of `0.768098`.