# MSCS 634 - Lab Assignment 2: KNN and RNN Classification on Wine Dataset

## Student Details
**Name:** Chandra Kiran Billingi  
**Course:** MSCS 634 – Machine Learning  
**Lab Title:** Classification Using KNN and RNN Algorithms
**Dataset:** Wine Dataset from scikit-learn

---

## 🔍 Purpose of the Lab

In this lab i have  explored and compared the performance of **K-Nearest Neighbors (KNN)** and **Radius Neighbors (RNN)** classifiers using the Wine dataset provided by scikit-learn. The primary objective  is to evaluate how the change in hyperparameters — `k` in KNN and `radius` in RNN — effects the classification accuracy. This comparison helped me in selecting optimal parameters and choosing the appropriate classifier for a given dataset.

---

## 📊 Key Insights from Accuracy Trends

- **KNN Classifier:**
  - Lower values of `k` (e.g., k=1 or k=5) provided me with a  better accuracy on the Wine dataset.
  - Accuracy generally decreased slightly with larger `k` mainly due to over-smoothing of the data set.
  - Best accuracy observed when the value of `k = 5`.

- **RNN Classifier:**
  - Accuracy was highly sensitive to the choice of radius.
  - If the radius was too small, some test points had no neighbors, resulting in errors or poor accuracy.
  - Larger radius values included too many neighbors, reducing precision.
  - Optimal performance observed at intermediate radius values (e.g., radius = 450).

- **Comparison:**
  - **KNN** was more stable and provided consistent performance.
  - **RNN** was more sensitive and required careful tuning to avoid prediction issues.

---

## ⚠️ Challenges Faced

- Handling errors with **RNN** when no neighbors were found within the specified radius for some test instances as i have a little experience in debugging machine learning codes so it took a sufficient amount of time to understand the root cause.
- Scaling features properly using `StandardScaler` was necessary to avoid distance-based bias.
- Deciding reasonable ranges for `radius` in RNN since its behavior was dataset-dependent and more erratic than KNN.

---



