# 5G User Prediction Project

## Project Overview

This project aims to predict whether a user is a 5G user based on their basic information and communication-related data such as call charges, data usage, activity behavior, package type, and region information. The project uses various machine learning algorithms to build predictive models and optimize their performance.

## Project Background

During the 2022 World Internet Conference Wuzhen Summit, the "World Internet Development Report 2022" indicated that in the first quarter of 2022, the global number of 5G users increased by 70 million, reaching approximately 620 million. According to Ericsson and GSMA, the global number of 5G users is expected to exceed 1 billion by the end of 2022. For telecom operators, it is helpful to create user profiles based on user-side information and make precise marketing efforts for potential 5G users.

## Data Description

The dataset contains 60 fields, with the `target` field being the prediction target. The main feature fields are divided into two categories: categorical (cat) and numerical (num) features. The dataset is available on the cloud platform, named `train.csv`.

### Feature Fields

- `id`: Sample identifier
- `cat_0` to `cat_19`: Categorical features
- `num_0` to `num_37`: Numerical features
- `target`: Target field, indicating whether the user is a 5G user

## Evaluation Metrics

The performance of the models is evaluated using the AUC (Area Under the Curve) metric. The higher the AUC score, the better the model performance.

## Algorithms and Optimization Techniques

### Initial Models

1. **Adaboosting**
2. **Decision Tree**
3. **K-means Clustering**
4. **KNN with FAISS**
5. **LightGBM**
6. **Logistic Regression**
7. **Naive Bayes**
8. **Random Forest**
9. **XGBoost**

### Optimization Techniques

1. **Grid Search**: Used in `KNN_Grid Search.ipynb`, `LightGBM_Grid Search.ipynb`, and `XGBoost_Hyperparameter Search.ipynb`.
2. **K Neighbors Change**: Used in `KNN_K_change.ipynb`, `KNN_K_n_neighbors_change.ipynb`, and `KNN_n_neighbors_change.ipynb`.
3. **Bayesian Optimization**: Used in `LightGBM_Bayes.ipynb` and `XGBoost_Bayes_3para.ipynb`.
4. **Particle Swarm Optimization (PSO)**: Used in `LightGBM_PSO.ipynb`.
5. **Feature Crosses**: Used in `XGBoost_Feature Crosses.ipynb`.
6. **Random Search with Early Stopping**: Used in `XGBoost_Random Search_Early Stopping.ipynb`.

## Repository Structure
│ ├── 5Gpredict_Adaboosting.ipynb
│ ├── 5Gpredict_DecisionTree.ipynb
│ ├── 5Gpredict_K-means.ipynb
│ ├── 5Gpredict_KNN_FAISS.ipynb
│ ├── 5Gpredict_LightGBM.ipynb
│ ├── 5Gpredict_LogisticRegression.ipynb
│ ├── 5Gpredict_NaiveBayes.ipynb
│ ├── 5Gpredict_Randomforest.ipynb
│ ├── 5Gpredict_XGBoost.ipynb
│ ├── KNN_Grid Search.ipynb

├── KNN
│ ├── KNN_K_change.ipynb
│ ├── KNN_K_n_neighbors_change.ipynb
│ ├── KNN_n_neighbors_change.ipynb

├── LightGBM
│ ├── LightGBM_Bayes.ipynb
│ ├── LightGBM_Grid Search.ipynb
│ ├── LightGBM_PSO.ipynb

├── XGBoost
│ ├── XGBoost_Feature Crosses.ipynb
│ ├── XGBoost_Hyperparameter Search.ipynb
│ ├── XGBoost_Bayes_3para.ipynb
│ ├── XGBoost_Random Search_Early Stopping.ipynb

├── data
│ └── train.csv (not included in this repository)

├── README.md

## How to Run

1. Clone the repository:

    ```bash
    git clone https://github.com/F4nc1est/5GUserPrediction.git
    ```

2. Navigate to the project directory:

    ```bash
    cd 5GUserPrediction
    ```

3. Run the Jupyter notebooks to see the modeling process and results:

    ```bash
    jupyter notebook
    ```

## Results and Analysis

The detailed results and analysis of each model, including performance comparisons and optimization effects, can be found in the respective Jupyter notebooks. The analysis includes the reasoning behind model selection, data analysis, model comparison, and potential improvement suggestions.

## Contributing

We welcome contributions to this project. Please create a pull request or open an issue to discuss any changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
