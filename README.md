# Fake-News-Detection
Machine learning-based NLP model to classify news articles as real or fake using TF-IDF and logistic regression.


This project aims to detect **fake news articles** using **Natural Language Processing (NLP)** and **Machine Learning**. It classifies a news statement as **real or fake** using text vectorisation (TF-IDF) and a **Logistic Regression** classifier.

---

## Project Overview

| Component             | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| 📄 Dataset            | News articles with text and labels (real/fake)                              |
| 🔍 Text Processing    | Tokenization, lowercasing, stop word removal, stemming                      |
| 📊 Feature Extraction | TF-IDF vectorization to convert text into numerical features                |
| 🤖 Model              | Logistic Regression for binary classification                               |
| 🧪 Evaluation         | Accuracy, Confusion Matrix, Precision, Recall, F1 Score                      |

---

## Key Technologies

| Technology            | Purpose                                                      |
|------------------------|--------------------------------------------------------------|
| **NLP (NLTK / re)**    | Preprocessing news headlines and content                     |
| **TF-IDF Vectorizer**  | Feature extraction from text (via `sklearn.feature_extraction.text`) |
| **Logistic Regression**| Classification algorithm used to predict fake or real news   |

---

## Project Structure
fake-news-detection/
│
├── fake_news_detection.ipynb # Jupyter notebook (main code)
├── dataset.csv # Dataset used (Kaggle or similar)
├── README.md # Project overview and usage
└── requirements.txt # Required Python packages


---

## Dataset

- Source: [Kaggle Fake News Dataset](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset)
- Columns typically include:
  - `title`, `text`, `label` (1 = fake, 0 = real)

---

## How to Run

Clone the repo:
git clone https://github.com/your-username/fake-news-detection.git
cd fake-news-detection

pip install -r requirements.txt

jupyter notebook fake_news_detection.ipynb

---

## Evaluation Metrics
Metric	Description
Accuracy	Percentage of correct predictions
Precision	Correctly predicted fake out of all predicted fake
Recall	Correctly predicted fake out of all actual fake
F1 Score	Harmonic mean of precision and recall
Confusion Matrix	Breakdown of TP, FP, FN, TN

## Results
- Achieved high accuracy on test data (~95%+)
- Good balance between precision and recall
- Logistic Regression was interpretable and effective

## Limitations
- The model may not generalize well to news from unknown sources
- No deep contextual understanding (e.g., sarcasm, nuanced misinformation)
- Based on static dataset (not connected to live news APIs)
