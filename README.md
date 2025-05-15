# 🧠 Smart Fake Review Detector for Amazon Products  
*A Real-World NLP + Machine Learning Project to Restore Trust in E-commerce*

## 🚀 Overview
Product reviews play a critical role in influencing buyer decisions.  
However, **fake and misleading reviews** are flooding online platforms, reducing transparency and trust.  
This project builds an **AI-powered system** that detects fake reviews based on content and behavioral signals using **Natural Language Processing (NLP)** and **Machine Learning**.

> 📌 Goal: Automatically classify reviews as **Fake ❌** or **Genuine ✅** to assist customers and platforms in making trusted decisions.

## 📂 Dataset
- Source: [Kaggle – Consumer Reviews of Amazon Products]
- Size: ~34,000 reviews
- Features used: `reviews.text`, `reviews.rating`, `reviews.numHelpful`, `reviews.username`

## ⚙️ Technology Stack

- **Python** (Jupyter/Kaggle Notebook)
- **NLP with NLTK**
- **TF-IDF Vectorizer**
- **Logistic Regression**
- **Matplotlib / Seaborn / WordCloud** for visualizations

## 🔨 Project Workflow
1. **Data Cleaning**: Removed noise, nulls, and preprocessed text
2. **Feature Engineering**: Added `text_length`, and helpfulness score
3. **Labeling**: Rule-based logic for identifying fake reviews
4. **Text Vectorization**: TF-IDF used to convert reviews into numeric form
5. **Model Training**: Logistic Regression with 80/20 split
6. **Evaluation**: Precision, Recall, F1-score, Confusion Matrix
7. **Visualization**: WordClouds, review length, rating distribution

## 📊 Visualizations Included
- Rating distribution
- Review length by label
- WordCloud for Fake and Genuine
- Top 15 words in Fake Reviews (Bar plot)

## 🧠 Model
- **TF-IDF** used to vectorize text
- **Logistic Regression** used for classification
- Accuracy: ~97%
- Evaluation metrics: Precision, Recall, F1-Score, Confusion Matrix

## 💡 Try It Yourself
```python
predict_review("This product is amazing, works great and I love it!")
# Output: ❌ Fake (Confidence: 89%)
