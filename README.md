# Amazon-Review-Analysis-ML
Final ML project analyzing Amazon review data using classification models.
# Amazon Review Analysis using Machine Learning

This project analyzes Amazon customer review data to evaluate the helpfulness and sentiment of product reviews. It was developed as part of a final milestone project for CSE 475.

## 📊 Dataset

- Source: `amazon.csv` (4915 rows × 12 columns)
- Includes: Reviewer names, review text, star ratings, votes, and derived metrics
- Unused: `Unnamed: 0` (index column)

## 🎯 Objective

To build a machine learning model that classifies or predicts review helpfulness based on structured customer review data. This includes both **classification** and **regression** possibilities.

## 🧹 Data Preprocessing

- Removed unnecessary features like:
  - `reviewerName`
  - `reviewText`
  - `reviewTime`
- Handled:
  - Missing values
  - Categorical encoding
  - Irrelevant columns

## 🧠 Models Used

1. **Random Forest Classifier**
   - Final model
   - Accuracy: `0.76`
2. **Logistic Regression**
3. **XGBoost Classifier**

### 📌 Note:
- Features such as `score_pos_neg_diff`, `score_average_rating`, and `wilson_lower_bound` were derived to help measure the quality of a review.
- Performance was measured using `accuracy`. Further evaluation (e.g. precision, recall, F1-score) is recommended for better understanding.

## 🧪 Results

- **Random Forest** provided the best performance.
- Identified challenges:
  - Overfitting risk
  - Linear limitations in Logistic Regression
  - Hyperparameter tuning in XGBoost

## 💡 Future Work

- Improve evaluation metrics (F1, AUC)
- Perform hyperparameter tuning
- Build an API or frontend to display review analytics

## 🛠️ Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
