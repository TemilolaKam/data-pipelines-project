# README Template


## Fashion Forward Forecasting

### Project Overview

StyleSense is a booming online women's clothing retailer experiencing exponential growth. As customer reviews pour in, many lack explicit feedback on whether the reviewer recommends the product. However, these reviews often contain valuable textual information that can be mined using NLP.

This project builds a machine learning pipeline that leverages structured (e.g., age, product category) and unstructured (text reviews) data to predict whether a customer would recommend a product. The end goal is to automate insights from incomplete reviews and help StyleSense stay on the cutting edge of fashion intelligence.

---

### Problem Statement

Due to a rapid increase in customer volume, StyleSense faces a challenge: many product reviews are missing the “recommend” label. Your task is to train a predictive model on the existing complete reviews to infer the missing ones. This enables:

* Better product insights
* Trend detection
* Enhanced customer satisfaction analysis



### Key Features Engineered

* **NLP-derived Features**:

  * TF-IDF vectors from review text
  

  * Age
  * Product category
  * Review length

---

### ML Pipeline Approach

1. **Data Preprocessing**:

   * Handling missing values
   * Standardizing numerical features (e.g., age)
   * One-hot encoding for categorical features
   * Text cleaning (lowercasing, punctuation removal, etc.)

2. **Feature Engineering**:

   * TF-IDF on review text
   

3. **Modeling**:

   * Trained classifiers: Logistic Regression
   * Evaluated using ROC-AUC, accuracy, precision, recall, and F1-score

4. **Pipeline Construction**:

   * Used `Pipeline` and `ColumnTransformer` from `sklearn`
   * Combined numerical, categorical, and text features into a single workflow

5. **Model Evaluation**:

   * ROC Curve
   * Confusion Matrix


### 🛠️ Libraries Used

* `pandas`, `numpy`
* `scikit-learn`
* `matplotlib`, `seaborn`



### 💡 Future Extensions

* Build a **Streamlit dashboard** to accept new reviews and return predictions.
* Improve text feature representation using transformer models (e.g., BERT).
* Add customer history and product metadata to enrich features.





## License

[License](LICENSE.txt)
