

***

# 📝 Customer Feedback Categorization using Clustering and NLP

***

## 📌 Project Overview
This project analyzes customer reviews—such as those from the Google Play Store—to uncover major feedback themes using clustering and NLP techniques. By processing, cleaning, and categorizing reviews with machine learning, it helps businesses:
- Understand user sentiment
- Surface frequent topics
- Identify areas needing improvement

***

## 📂 Data Sources
- **Play Store App Data**: App titles, categories, ratings, installs, and other metadata
- **User Reviews**: Feedback text (including translated reviews for sentiment analysis)

***

## 🔍 Main Steps

1. **Data Cleaning** 🧹
    - Drop missing values from critical columns
    - Normalize text fields (lowercase, remove whitespace)
    - Detect and remove outliers in numerical columns

2. **Preprocessing** 🏗️
    - One-hot encode categorical features (like app category)
    - Scale numerical features (rating, reviews, installs, price)
    - Clean review text using NLP (stopword removal, lemmatization)

3. **Feature Engineering** 🛠️
    - TF-IDF vectorization for review text
    - Sentiment analysis scores (polarity, subjectivity)

4. **Clustering** 🧩
    - KMeans used to find groups of similar feedback
    - Cluster quality assessed with Silhouette Score, Calinski-Harabasz, and Davies-Bouldin Index

5. **Analysis** 📊
    - Characterize each cluster by sentiment, keywords, and sample review text

***

## 🧑‍💻 Algorithms and Techniques

- NLTK for word cleaning and normalization
- scikit-learn for clustering, feature engineering, and evaluation
- TF-IDF for keyword extraction
- Sentiment analysis for qualitative insights

***

## 💡 Sample Results

Three main clusters frequently emerge:
- ❗ Negative/Issue Focused: Complaints and problem reports
- ℹ️ Low Positive/Informational: Neutral or mildly positive feedback
- 🌟 High Positive/Enthusiastic: Highly positive, enthusiastic reviews

***

## 🏆 Evaluation Metrics

- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index

***

## ⚙️ How to Run

1. 🔽 Clone the repository and install dependencies from `requirements.txt`
2. 🗃️ Place `Play Store Data.csv` and `User Reviews.csv` in the working directory
3. 📓 Run `data.ipynb` in Jupyter Notebook or VS Code
4. 📈 Review cluster assignments and analysis in notebook output

***

## 🧩 Dependencies

- Python 3.9+
- pandas
- numpy
- scikit-learn
- NLTK
