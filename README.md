#  Email Spam Detection using Machine Learning (Internship project 1)

An end-to-end Machine Learning project designed to classify emails as either **Spam (1)** or **Ham / Legitimate (0)**. This project explores data preprocessing, text vectorization (TF-IDF), model training across multiple algorithms, and performance evaluation.

---

##  Project Overview

Spam emails pose security threats, phishing risks, and inbox clutter. The goal of this project is to build an accurate classification pipeline using traditional Machine Learning models and tree-based ensembles to effectively filter unwanted communications.

* **Dataset:** Kaggle - [Spam Email Dataset](https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)
* **Dataset Size:** 5,728 email records (`text` and `spam` label)
* **Supervisor:** Sk Asrafuzzaman (Head Lecturer, ICT)

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.12+
* **Data Processing:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`, `dtreeviz`
* **Machine Learning:** `scikit-learn`, `xgboost`
* **Data Retrieval:** `opendatasets`

---

##  Repository Structure

```text
├── Spamdetection.ipynb   # Main Google Colab notebook
├── README.md             # Project documentation
└── dataset/              # Downloaded email dataset (emails.csv)

1. Data Collection & Setup
Environment set up in Google Colab.

Dataset automatically fetched using Kaggle API via opendatasets.

2. Preprocessing & Text Vectorization
Cleaned raw email text by removing header prefixes (e.g., Subject:).

Converted raw text strings into numerical representations using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization with English stop-word removal.

3. Model Training & Comparison
The project evaluates several classification algorithms:

Naive Bayes (GaussianNB, MultinomialNB)

Logistic Regression

Decision Trees & Random Forest

Support Vector Machines (SVM)

XGBoost Classifier (XGBClassifier)

4. Evaluation Metrics
Models are evaluated on:

Accuracy

Precision & Recall

F1-Score

Confusion Matrix & ROC-AUC Curves

---

## 📚 References & Resources

### Dataset & Supervisor
* **Dataset:** CSIC Spam Email Dataset via Kaggle — [jackksoncsie/spam-email-dataset](https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)
* **Project Guidance:** Project structured under the supervision of **Sk Asrafuzzaman** (Head Lecturer, ICT).

### Libraries & Frameworks
* **Scikit-Learn:** Pedregosa et al., *Scikit-learn: Machine Learning in Python*, JMLR 12, pp. 2825-2830, 2011. — [https://scikit-learn.org](https://scikit-learn.org)
* **XGBoost:** Chen, T., & Guestrin, C. (2016). *XGBoost: A Scalable Tree Boosting System*. In Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (pp. 785–794). — [https://xgboost.readthedocs.io](https://xgboost.readthedocs.io)
* **dtreeviz:** Visualizing Decision Trees and Decision Boundaries — [https://github.com/parrt/dtreeviz](https://github.com/parrt/dtreeviz)
* **Pandas & NumPy:** McKinney, W. (2010). *Data Structures for Statistical Computing in Python*. Proceedings of the 9th Python in Science Conference, pp. 56-61.

### Algorithmic Background
* **TF-IDF & Text Mining:** Salton, G., & Buckley, C. (1988). *Term-weighting approaches in automatic text retrieval*. Information Processing & Management, 24(5), 513-523.
* **Naive Bayes for Spam Filtering:** Sahami, M., Dumais, S., Heckerman, D., & Horvitz, E. (1998). *A Bayesian approach to filtering junk e-mail*. AAAI Workshop on Learning for Text Categorization.
