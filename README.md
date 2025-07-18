# Kaggle


## Project 1: E-Commerce CRM Analytics & Retention Pipeline
A comprehensive end-to-end solution for merging, cleaning, and analyzing e-commerce CRM data to uncover customer retention, repeat-purchase behavior, churn, and product performance—and to generate dashboard-ready datasets for Looker Studio.

**Project Overview**
This project ingests raw sales and retention CSV exports, cleans and preprocesses the data, computes key customer metrics (YoY & MoM retention, repeat purchase rates, churn), and produces a suite of analytics datasets—cohort tables, performance summaries, SKU rankings, and KPI reports. All outputs are optimized for fast loading into BI tools.

**Key Features**

**Data Merging & Cleaning**  
  - Concatenate multiple sales exports  
  - Standardize date fields, email addresses, segments  
  - Handle missing or invalid values  

**Retention & Repurchase Metrics**  
  - Year-over-Year & Month-over-Month retention rates  
  - Repeat purchase rate (1st→2nd and dynamic per period)  
  - Churn rate calculation (90-day inactivity)  

**Analytics Datasets**  
  - **Customer Analytics**: CLV, order frequency, segments  
  - **Cohort Analysis**: month-based retention curves  
  - **Monthly & Quarterly Performance**: orders, revenue, AOV, completion rates  
  - **Product/SKU Insights**: top SKUs by period, repurchase rates  
  - **New vs. Repeat Customers**: Excel report with separate sheets  

**KPI Summary & Dashboard Prep**  
  - High-level KPIs (total customers, retention, churn, revenue, AOV)  
  - Data dictionaries for every CSV  
  - Optimized “small & fast” exports for Looker Studio  
  - Sample datasets for rapid prototyping  

**Project Links**
- **Kaggle Notebook:** https://www.kaggle.com/code/ahmadulkc/ecommerce-data-analysis/
- **Looker Studio Dashboard:** https://lookerstudio.google.com/reporting/61ad4d20-c9e4-4808-8b94-62cc1617b3e2/

![eCommerce_Analytics_Dashboard_page-0001](https://github.com/user-attachments/assets/72ed3f40-4b2f-4135-a87b-9a1cd5bfb799)






## Project 2: Suicidal Thought Detection (KNN, SVM, Decision Tree, Multinomial Naive Bayes)
This script explores different techniques for building a model to classify text data into suicidal or non-suicidal categories. Here's a summary of the key steps involved:

* Project File: [Kaggle](https://www.kaggle.com/code/ahmadulkc/suicide-thought-detection-knn-svm-dt-nb/notebook/), [GitHub](https://github.com/AKC23/Kaggle/blob/main/Projects/Suicidal%20Thought%20Detection%20(KNN%2C%20SVM%2C%20DT%2C%20NB).ipynb)
* Dataset: [Suicide and Depression Detection](https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch/data/)

**Data Loading and Preprocessing:**
* Reduces the dataset size to 10,000 entries for faster processing.
* Converts all text to lowercase.
* Removes punctuation marks.
* Tokenizes the text data by splitting it into individual words.
* Removes stop words (common words like "the", "a", "an") from the vocabulary.

**Data Splitting:**

Splits the preprocessed data into training and testing sets using an 80:20 ratio.
The training set is used to train the model, and the testing set is used to evaluate the model's performance.

**Feature Extraction with CountVectorizer:**

CountVectorizer is used to transform text data into numerical features.
It counts the occurrences of each word in the text data.

**Experiments with different n-gram options:**
* Unigrams (single words)
* Bigrams (word pairs)
* Trigrams (three-word sequences)

**Model Building and Evaluation:**

Evaluates different machine learning models for sentiment classification:
1. Support Vector Machine (SVM)
1. Multinomial Naive Bayes (NB)
1. Decision Tree (DT)
1. K-Nearest Neighbors (KNN)

> Uses pipelines to combine feature extraction (CountVectorizer) with Tfidf transformation and the machine learning models. Trains each model on the training set and evaluates its performance on the testing set using accuracy score.

Overall, the script explores various feature engineering and machine learning techniques to identify the best approach for classifying text data into suicidal and non-suicidal categories.
<hr>





