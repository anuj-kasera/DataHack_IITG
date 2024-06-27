# DataHack_IITG

<h2>Overview</h2>

This project aims to develop a predictive model to classify individuals' vaccination status using demographic, behavioral, and opinion-related features. The model predicts two outcomes: xyz_vaccine and seasonal_vaccine.

<h2>Dataset</h2>

**Source:** The datasets used include training_set_features.csv (features data), training_set_labels.csv (target labels), and test_set_features.csv (unlabeled test data).

**Preprocessing:** Data cleaning involved removing irrelevant columns, imputing missing values (KNN Imputer for numerical, 'Missing' category for categorical), and encoding categorical variables using Label Encoding.

<h2>Feature Engineering</h2>

**Exploration:** Explored feature correlations using heatmap visualization and selected relevant features for modeling.

**Transformation:** Prepared the data for modeling by splitting into features (input1) and targets (target).

<h2>Modeling</h2>

**Algorithms:** Implemented several classifiers using MultiOutputClassifier:
Logistic Regression, Naive Bayes (Gaussian and Multinomial), SVC, Decision Trees, Random Forest, AdaBoost, Gradient Boosting, XGBoost, K-Nearest Neighbors.

**Hyperparameter Tuning:** Utilized RandomizedSearchCV to optimize the Gradient Boosting Classifier's parameters for improved performance.

<h2>Evaluation</h2>

**Metrics:**  Evaluated models based on ROC AUC score and accuracy on both training and test datasets.

**Best Model:** Selected Gradient Boosting Classifier based on highest ROC AUC score:
**ROC AUC Score (Train Data): 0.757
ROC AUC Score (Test Data): 0.744**

<h2>Conclusion</h2>

**Achievements:** Successfully developed and optimized a multilabel classifier to predict vaccination status, demonstrating robust performance in healthcare analytics.
**Next Steps:** Future work may involve further model refinement, deployment for real-time predictions, and integration into broader healthcare systems.
