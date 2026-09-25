# Statistics & Quantitative Methods for Data Science
### Course Overview — 8-Week Program

## What this course covers

This is an 8-week, project-based course covering statistics, probability, and machine learning for data science — from descriptive statistics through to ensemble methods and unsupervised learning, taught almost entirely through hands-on Jupyter notebooks built around a small set of real, running datasets (Titanic, and later a diamonds-pricing and penguin-species dataset for the capstone projects).

Each week runs **2 classes**. Across the 8 weeks, learners complete:

- **7 Labs** — one per week for Weeks 1-7, giving hands-on practice with that week's concepts using NumPy, pandas, Matplotlib, Seaborn, and SciPy.stats. (Week 8 has no new lab — it's dedicated project time.)
- **3 Projects** — the course's major applied deliverables:
  1. **N-grams project** (starts Week 3, right after the Week 2 probability course) — building N-gram language models, extending the probability and Bayes' theorem foundations into a small language-modelling project.
  2. **Regression project** (Week 8, Class 1) — a full regression pipeline applied to a dataset of the learner's own choosing.
  3. **Classification project** (Week 8, Class 2) — a full classification pipeline applied to a dataset of the learner's own choosing.

## Week-by-week structure

| Week | Class 1 | Class 2 |
|---|---|---|
| **1** | Intro to Statistics, Types of Data, Python for Data Science | Descriptive Statistics & Data Visualization (NumPy, pandas, Matplotlib) |
| **2** | Probability Theory, Bayes' Theorem & N-gram Language Models | Probability Distributions, Sampling Techniques & the Central Limit Theorem |
| **3** | Inferential Statistics & Confidence Intervals | Hypothesis Testing, p-values & Statistical Significance |
| **4** | Exploratory Data Analysis & Correlation | Simple & Multiple Linear Regression |
| **5** | Statistical Methods for ML & Feature Selection | Classification Algorithms (Logistic Regression, KNN, Decision Trees) |
| **6** | Bias-Variance Tradeoff & Regularization (Ridge, Lasso, ElasticNet) | Model Evaluation Metrics & A/B Testing |
| **7** | Ensemble Methods (Random Forests, Gradient Boosting) | Unsupervised Learning (K-Means Clustering & PCA) |
| **8** | **Regression Project** — peer learning + instructor guidance | **Classification Project** — peer learning + instructor guidance |

**Note on Weeks 1-3**: these carry over unchanged from the original 6-week syllabus.

**Note on Weeks 4-7**: these expand the original Weeks 4-5 ("Correlation/Regression/EDA" and "Statistical Methods for ML/A-B Testing") from 2 weeks into 4, adding classification algorithms, the bias-variance tradeoff, regularization, ensemble methods, and unsupervised learning — core data science topics not in the original outline.

**Note on Week 8**: this replaces the original Week 6 capstone/portfolio week. Rather than a single guided project, Week 8 is now two full peer-learning sessions where learners build their Regression and Classification projects, each with 5 linked top Kaggle projects for inspiration and a fully worked example pipeline (on a dataset different from the learner's own) to model their own project on.

## The 3 projects, in brief

1. **N-grams (Week 3)**: applies Week 2's probability and Bayes' theorem content — building unigram/bigram/trigram language models with Laplace smoothing, generating text, and (optionally) using an N-gram model as the likelihood inside a Naive Bayes-style text classifier.
2. **Regression (Week 8, Class 1)**: learners pick their own regression dataset and run it through the full pipeline demonstrated in class on the `diamonds` dataset — EDA, feature engineering, a baseline linear model, a regularized/ensemble model, and honest cross-validated evaluation.
3. **Classification (Week 8, Class 2)**: same structure, for a classification problem of the learner's choosing, demonstrated in class on the `penguins` dataset.

All 3 projects end with a short written statistical report (Question → Method → Findings → Caveats → Recommendation) and are meant to become portfolio pieces.
