# Customer Dispute Prediction & Dashboard

##  Introduction

This project aims to predict whether a customer will dispute an issue with the bank using a combination of data analysis, machine learning models, and dashboard visualization. By leveraging Python for preprocessing and Power BI for reporting, we provide a complete pipeline from raw data to business-ready insights.

---

##  Objectives

- Predict whether a customer will dispute a complaint (`Consumer disputed?`) using machine learning.
- Perform comprehensive data analysis and visualization in Python.
- Build and evaluate multiple classification models to find the best-performing one.
- Save predictions for business decision-making.
- Create an interactive Power BI dashboard for stakeholder insights.

---

##  Dataset Description

The dataset contains detailed records of customer complaints submitted to banks. Key features include:

| Feature | Description |
|--------|-------------|
| `Date received` | Date complaint was received |
| `Product`, `Sub-product` | Type and sub-type of financial product |
| `Issue` | Description of the customer’s complaint |
| `Company public response` | Company's formal response |
| `Company` | The financial institution's name |
| `State`, `ZIP code` | Customer location |
| `Submitted via` | Submission channel (web, phone, etc.) |
| `Date sent to company` | Date complaint was forwarded to the company |
| `Timely response?` | Whether the company responded on time |
| `Consumer disputed?` | **Target variable** |
| `Complaint ID` | Unique identifier |

---

##  Methodology

### 🔧 Data Preparation

- Imported libraries: `pandas`, `numpy`, `seaborn`, `matplotlib`, `sklearn`, `nltk`, etc.
- Loaded the dataset and handled missing values.
- Encoded categorical variables and cleaned textual fields like `Issue`.

###  Text Preprocessing

- Tokenized, removed stopwords, and cleaned complaint descriptions using NLP (NLTK).
- Extracted features to improve model accuracy.

###  Exploratory Data Analysis (EDA)

- Visualized age, gender, and complaint issue distributions.
- Binned `Age` into groups and created state-wise summaries.
- Analyzed patterns in timely responses and disputes.

---

## Model Building

Multiple models were trained and evaluated:

- Logistic Regression ✅ **(Best performance)**
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- AdaBoost Classifier
- Gradient Boosting Classifier
- XGBoost Classifier


---

##  Power BI Dashboard

An interactive dashboard (`dashboard.pbix`) was created with:

- Complaint volume over time
- Timely vs untimely responses
- Funnel chart for complaint resolution stages:
  `Received → Sent to Company → Timely → Resolved`
- Age & Gender distributions
- Top products and issues
- And more...

> The Power BI dashboard enables business users to interactively explore the complaints data and model predictions.
![image](https://github.com/user-attachments/assets/32acffb1-9104-4731-81d4-161d7ec1dfde)
![image](https://github.com/user-attachments/assets/a0d2088e-056d-47ee-87b9-54a31ad9f03b)






---


