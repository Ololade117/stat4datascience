# Machine Learning Projects — Kaggle Practice Set

This project set is designed for learners who have finished the basic Machine Learning Concepts material and need practical projects to apply the workflow.

There are **6 projects**:

- **3 Supervised Learning projects** — the dataset provides a target that the model must predict.
- **3 Unsupervised Learning projects** — there is no prediction target; the goal is to discover structure in the data.

The projects deliberately cover different types of data-science problems rather than repeating the same task five times.

---

# Part I — Supervised Learning Projects

## Project 1 — House Prices: Predict House Sale Prices

**Learning type:** Supervised Learning  
**Problem type:** Regression  
**Level:** Beginner → Intermediate

### Kaggle
[House Prices — Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

### Project question
> Can we predict the sale price of a house from information describing the property?

The competition provides many explanatory variables describing homes in Ames, Iowa and asks participants to predict `SalePrice`. Kaggle explicitly highlights feature engineering, random forests, and gradient boosting as useful skills for the competition. [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

### What students should practice

- Regression problem formulation
- Understanding numerical and categorical features
- Missing-value analysis
- Feature distributions and outliers
- Feature engineering
- Log transformations
- One-hot encoding
- Scaling where appropriate
- Linear Regression and regularized linear models
- Decision Trees and Random Forests
- Gradient boosting
- MAE, RMSE, and R²
- Cross-validation
- Comparing a simple model with a more flexible model

### Suggested workflow

1. Load `train.csv` and inspect the dataset.
2. Identify `SalePrice` as the target.
3. Examine the target distribution.
4. Investigate missing values and distinguish meaningful missingness from data errors.
5. Explore important relationships with the target.
6. Build a preprocessing pipeline.
7. Establish a simple regression baseline.
8. Train a linear model.
9. Train a Random Forest.
10. Try a boosting model.
11. Use cross-validation to compare models.
12. Perform targeted feature engineering.
13. Generate Kaggle predictions.

### Deliverables

- Exploratory data analysis
- Missing-value strategy
- Baseline model
- At least three model experiments
- Cross-validation results
- Feature-engineering section
- Final Kaggle submission
- Written discussion of which features and modeling decisions affected performance

### Extension
Study whether a simpler feature set generalizes as well as a heavily engineered feature set. Keep the test set untouched while making modeling decisions.

---

## Project 2 — Medical Cost Prediction

**Learning type:** Supervised Learning  
**Problem type:** Regression  
**Level:** Beginner → Intermediate

### Kaggle
[Medical Cost Personal Datasets](https://www.kaggle.com/mirichoi0218/insurance)

### Project question
> Can we predict an individual's medical insurance charges from demographic and health-related information?

The Kaggle dataset contains 1,338 observations and variables including age, sex, BMI, number of children, smoking status, region, and medical charges. The task naturally becomes a regression problem because `charges` is a numerical target. Kaggle also provides multiple community notebooks using this dataset for exploratory analysis and linear regression.

### What students should practice

- Regression problem formulation
- Numerical and categorical feature analysis
- Exploratory data analysis
- Missing-value and data-quality checks
- One-hot encoding
- Feature scaling where appropriate
- Linear Regression
- Regularized regression
- Decision Trees and Random Forests
- MAE, RMSE, and R²
- Residual/error analysis
- Cross-validation
- Feature interpretation

### Suggested workflow

1. Load the dataset and inspect its shape, types, and summary statistics.
2. Identify `charges` as the target.
3. Explore how charges vary with age, BMI, children, smoking status, and region.
4. Check missing values, duplicates, outliers, and unusual values.
5. Separate numerical and categorical features.
6. Build a preprocessing pipeline.
7. Establish a simple mean baseline.
8. Train Linear Regression.
9. Train a regularized linear model such as Ridge.
10. Try a tree-based regression model.
11. Evaluate using MAE, RMSE, and R².
12. Inspect residuals and difficult predictions.
13. Use cross-validation to compare approaches.
14. Explain which features appear associated with higher or lower predicted charges, without treating association as proof of causation.

### Deliverables

- Exploratory data analysis
- Data-quality report
- Preprocessing pipeline
- Baseline model
- At least three regression experiments
- Metric comparison
- Residual/error analysis
- Cross-validation results
- Short interpretation of important relationships and limitations

### Extension
Compare a purely linear model with a nonlinear tree-based model. Investigate which types of observations account for the largest prediction errors.

---

## Project 3 — Telco Customer Churn Prediction

**Learning type:** Supervised Learning  
**Problem type:** Binary Classification  
**Level:** Beginner → Intermediate

### Kaggle
[Telco Customer Churn Dataset](https://www.kaggle.com/datasets/abbas829/telco-customer-churn-dataset)

### Project question
> Can we predict whether a telecommunications customer is likely to churn based on their demographic, service, contract, and billing information?

The Kaggle dataset describes customers of a fictional telecommunications company and includes customer demographics, account information, subscribed services, and a binary `Churn` target indicating whether the customer left. Kaggle identifies it as a binary-classification dataset. [Kaggle](https://www.kaggle.com/datasets/abbas829/telco-customer-churn-dataset)

### What students should practice

- Classification problem formulation
- Numerical and categorical feature analysis
- Missing-value handling
- One-hot encoding
- Feature scaling
- Class distribution analysis
- Logistic Regression
- Decision Trees and Random Forests
- Precision, recall, F1, and accuracy
- Confusion matrices
- Probability predictions and classification thresholds
- Cross-validation
- Error analysis
- Basic model interpretation

### Suggested workflow

1. Load the dataset and inspect the columns.
2. Identify `Churn` as the target.
3. Examine class balance.
4. Explore numerical and categorical variables.
5. Check missing values and data quality.
6. Build a preprocessing pipeline for numerical and categorical features.
7. Establish a simple classification baseline.
8. Train Logistic Regression.
9. Train a tree-based model.
10. Evaluate using a confusion matrix, precision, recall, F1, and accuracy.
11. Compare the models using cross-validation.
12. Investigate examples the model gets wrong.
13. Examine whether changing the classification threshold affects precision and recall.

### Deliverables

- Exploratory data analysis
- Data-cleaning and preprocessing strategy
- Class-distribution analysis
- Baseline classifier
- At least two model experiments
- Confusion matrix
- Precision, recall, F1, and accuracy results
- Cross-validation comparison
- Error analysis
- Short explanation of the most useful features and important limitations

### Extension
Investigate how the choice of probability threshold changes the trade-off between catching likely churners and generating false alarms. Discuss which metric would matter most for a hypothetical retention campaign.

# Part II — Unsupervised Learning Projects

## Project 4 — Mall Customer Segmentation

**Learning type:** Unsupervised Learning  
**Problem type:** Clustering  
**Level:** Beginner

### Kaggle
[Mall Customer Segmentation Data](https://www.kaggle.com/datasets/PromptCloudHQ/mall-customers-segmentation)

A useful Kaggle notebook based on this dataset demonstrates customer segmentation with K-Means and explores customer groups using variables such as age, annual income, and spending score. [Kaggle notebook](https://www.kaggle.com/code/listonlt/mall-customers-segmentation-k-means-clustering)

### Project question
> Can we group customers into meaningful segments based on their characteristics and spending behavior?

Unlike supervised learning, there is no target such as “customer segment.” The clustering algorithm must discover groups from the available features.

### What students should practice

- Understanding unsupervised learning
- Exploratory data analysis without a target
- Feature selection for clustering
- Feature scaling
- Distance-based similarity
- K-Means clustering
- Choosing a reasonable number of clusters
- Elbow method
- Silhouette score
- Cluster visualization
- Cluster profiling
- Interpreting clusters cautiously

### Suggested workflow

1. Load the customer dataset.
2. Inspect numerical and categorical variables.
3. Decide which variables should be used for clustering.
4. Scale the selected variables.
5. Visualize the data.
6. Run K-Means for several values of `k`.
7. Use the elbow method and silhouette score as supporting evidence.
8. Fit the selected clustering model.
9. Summarize each cluster using descriptive statistics.
10. Give each cluster a descriptive business-oriented name only after inspecting its characteristics.

### Deliverables

- EDA notebook
- Justification for chosen clustering features
- Elbow plot
- Silhouette analysis
- Cluster visualization
- Cluster summary table
- Business interpretation of each cluster
- Discussion of limitations

### Extension
Try PCA to visualize the clusters in two dimensions and compare the visualization with the original feature space.

---

## Project 5 — Wholesale Customer Segmentation

**Learning type:** Unsupervised Learning  
**Problem type:** Clustering  
**Level:** Beginner → Intermediate

### Kaggle
[Wholesale Customers Data Set](https://www.kaggle.com/binovi/wholesale-customers-data-set/kernels)

The Kaggle dataset contains annual spending information for clients of a wholesale distributor. [Kaggle](https://www.kaggle.com/binovi/wholesale-customers-data-set/kernels)

### Project question
> Can we discover groups of wholesale customers that have different purchasing patterns?

This project moves beyond a tiny teaching dataset and gives students several spending variables that can be used to identify customer profiles.

### What students should practice

- Clustering with multiple numerical features
- Data distributions and skewness
- Log transformations where appropriate
- Scaling
- K-Means
- Hierarchical clustering
- Distance and similarity
- Dendrograms
- Silhouette score
- Comparing clustering methods
- Interpreting segments using summary statistics

### Suggested workflow

1. Load and inspect the dataset.
2. Understand every spending variable.
3. Check for strong skewness and outliers.
4. Consider appropriate transformations.
5. Standardize the features.
6. Apply K-Means.
7. Test several values of `k`.
8. Apply hierarchical clustering.
9. Compare the resulting structures.
10. Profile each cluster.
11. Explain what different purchasing patterns could mean for the distributor.

### Deliverables

- EDA
- Feature-distribution analysis
- Preprocessing decisions
- K-Means analysis
- Hierarchical clustering analysis
- Cluster comparison
- Visualizations
- Cluster profiles and interpretation

### Extension
Investigate how the clusters change when one high-variance feature is removed. Discuss whether a cluster is robust to changes in feature selection.

---

## Project 6 — Fashion MNIST with PCA

**Learning type:** Unsupervised Learning  
**Problem type:** Dimensionality Reduction / PCA  
**Level:** Beginner → Intermediate

### Kaggle
[Fashion MNIST](https://www.kaggle.com/zalando-research/fashionmnist)  
[PCA for Fashion MNIST Classification](https://www.kaggle.com/competitions/pca-for-fashion-mnist-classification/data)

### Project question
> Can we reduce the dimensionality of Fashion MNIST images while retaining as much useful variation as possible?

Fashion MNIST contains 70,000 grayscale images, each with 28 × 28 pixels, which means each image can be represented by 784 pixel features. Kaggle also hosts a dedicated PCA competition based on Fashion MNIST. In this project, **PCA itself should be treated as the unsupervised task**: do not use the clothing labels when fitting PCA. Labels may be used afterward only for optional visualization or analysis.

### What students should practice

- Understanding high-dimensional data
- Feature scaling and centering
- Covariance and variance intuition
- Principal Component Analysis (PCA)
- Explained variance ratio
- Cumulative explained variance
- Choosing the number of components
- Transforming data into principal-component space
- 2D and 3D visualization
- Reconstruction and information loss
- Interpreting PCA loadings
- Comparing original and reduced representations

### Suggested workflow

1. Load a manageable portion of the Fashion MNIST training data initially.
2. Inspect the image shape and pixel-value range.
3. Reshape each 28 × 28 image into a 784-dimensional feature vector.
4. Standardize or otherwise appropriately center the feature representation.
5. Fit PCA without using the image labels.
6. Plot the explained variance ratio for the first components.
7. Plot cumulative explained variance.
8. Choose several possible values of `n_components`.
9. Transform the images into their lower-dimensional representations.
10. Visualize observations using the first two principal components.
11. Optionally use the known clothing labels only to color the visualization and ask whether classes appear separated in PCA space.
12. Reconstruct selected images from a small number of components.
13. Compare reconstruction quality as the number of components increases.
14. Discuss the trade-off between dimensionality reduction and information loss.

### Deliverables

- Explanation of why the raw data is high-dimensional
- Data-preprocessing decisions
- Explained-variance plot
- Cumulative explained-variance plot
- 2D PCA visualization
- Comparison of several component counts
- Original-versus-reconstructed image examples
- Short discussion of information loss
- Interpretation of major components/loadings

### Extension
Compare PCA using 2, 10, 50, and 100 components. Measure how much variance each representation retains and visually inspect how reconstruction changes. Then discuss why retaining more variance does not necessarily mean that every downstream task will perform better.

---

# Recommended Project Order

For a beginner class, the projects can be completed in this order:

| Order | Project | Learning Type | Main Skill |
|---|---|---|---|
| 1 | Mall Customer Segmentation | Unsupervised | K-Means clustering |
| 2 | Medical Cost Prediction | Supervised | Regression + preprocessing |
| 3 | Telco Customer Churn | Supervised | Classification + evaluation metrics |
| 4 | House Prices | Supervised | Regression + feature engineering |
| 5 | Wholesale Customer Segmentation | Unsupervised | Clustering comparison |
| 6 | Fashion MNIST with PCA | Unsupervised | Dimensionality reduction |

This order introduces clustering first, then supervised regression and classification, before moving into a more demanding regression dataset, clustering comparison, and finally high-dimensional dimensionality reduction.

---

# Minimum Requirements for Every Project

Every student project should contain these sections in the notebook:

1. **Problem Definition** — What question are you answering?
2. **Dataset Description** — What does each important variable mean?
3. **Data Inspection** — Shape, data types, missing values, duplicates, and basic statistics.
4. **EDA** — At least several meaningful visualizations.
5. **Preprocessing** — Explain every important cleaning/transformation decision.
6. **Baseline** — Establish a simple reference where applicable.
7. **Modeling** — Train at least two reasonable approaches where the task allows it.
8. **Evaluation** — Use metrics appropriate to the problem.
9. **Error/Cluster Analysis** — Investigate mistakes or discovered groups rather than looking only at a final score.
10. **Conclusion** — Explain what was learned, what worked, what did not, and what limitations remain.

---

# Important Practice Rules

### Rule 1 — Understand the problem before modeling

Do not begin with “Which algorithm should I use?” Begin with “What question am I trying to answer?”

### Rule 2 — Keep evaluation data separate

Do not repeatedly use the final test set to make modeling decisions.

### Rule 3 — Watch for data leakage

Any information that would not be available when making the real prediction should not enter the training process.

### Rule 4 — Explain preprocessing

Do not simply call `dropna()`, `StandardScaler()`, or one-hot encoding. Explain why the operation is appropriate.

### Rule 5 — A score is not the whole project

A good data-science project explains the data, assumptions, methods, results, errors, and limitations.

### Rule 6 — For unsupervised learning, do not force an interpretation

Clusters are mathematical groupings produced under a particular representation and algorithm. Profile them using evidence rather than assuming they are naturally occurring categories.

---

# Final Project Goal

By completing all six projects, a student should have practiced the core data-science loop across several settings:

**Understand the problem → Understand the data → Clean → Explore → Prepare → Model → Evaluate → Interpret → Communicate**

The objective is not to maximize Kaggle leaderboard performance. The objective is to develop the ability to build a complete, defensible machine-learning workflow.
