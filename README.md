# Fake-News-Detection


## The Problem

The rise of fake news has created a global challenge, impacting elections, public opinions, and overall trust in information sources. Fake news refers to fabricated stories with no verifiable facts, sources, or quotes, often spreading false information for political, economic, or social agendas. With the rise of automated bots, misinformation spreads rapidly, making it harder to distinguish between real and fake news.

To combat this, we need better systems that analyze patterns in fake news and improve media literacy, communication, and information reliability.

## Purpose

This project aims to detect fake news using machine learning techniques. It processes and analyzes collected data from news articles to classify them as real or fake. The goal is to build and evaluate machine learning models that can accurately distinguish between reliable and unreliable news sources.

## Dataset

The dataset is sourced from Kaggle: [Fake and Real News Dataset](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset)

It consists of two CSV files:

- `Fake.csv` - Contains 23,481 fake news articles.
- `True.csv` - Contains 21,417 real news articles.
- These datasets are merged into a single dataframe and labeled with a `target` column indicating "fake" or "true".
## Data Preprocessing

- **Data Cleaning:** Removing null values, unnecessary columns (like `date` and `title`).
- **Text Preprocessing:** Tokenization, stopword removal, and TF-IDF vectorization.
- **Splitting Dataset:** Train-test split for model evaluation.

## Exploratory Data Analysis (EDA)

- Checked dataset size and balance between fake and true news.
- Visualized data distributions using `matplotlib` and `seaborn`.

## Models Used

Multiple machine learning models are implemented:

1. **Logistic Regression** - A simple yet effective model for classification.
2. **Decision Tree Classifier** - A tree-based model that splits data based on feature importance.
3. **Random Forest Classifier** - An ensemble learning method that improves accuracy.

## Evaluation Metrics

The models are evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score

## Future Improvements

- Implementing deep learning models (LSTMs, Transformers) for better accuracy.
- Improving dataset quality by integrating more news sources.