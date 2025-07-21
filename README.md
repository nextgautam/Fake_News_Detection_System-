# 📰 Fake News Detection Using Machine Learning

This project is a machine learning-based solution for detecting fake news articles using natural language processing and classification algorithms. The goal is to automatically classify news content as **real** or **fake**, thereby combating the spread of misinformation.

---

## 👨‍💻 Author

**Gautam Yadav**  
📧 [gautamyadav1406@gmail.com](mailto:gautamyadav1406@gmail.com)  
📅 Project Date: July 9, 2025

---

## 📌 Project Objective

To build a binary text classification model that distinguishes between **fake** and **real** news based on the news article content using supervised learning techniques.

---

## 📁 Dataset Description

Two CSV files were used for training and testing:

- `Fake.csv`: Contains fake news articles
- `True.csv`: Contains legitimate news articles

Each file includes the following features:

- `title`: Headline of the news article
- `text`: Full text of the article
- `subject`: News category
- `date`: Date of publication  
- `class`: Added during preprocessing (`0` = Fake, `1` = True)

---

## 🧹 Data Preprocessing

- Merged fake and true news datasets
- Removed unnecessary columns (`title`, `subject`, `date`)
- Cleaned the text (punctuation, digits, links, HTML tags)
- Applied custom preprocessing using regular expressions
- Balanced and shuffled the dataset for training

---

## 📊 Feature Extraction

- Used **TF-IDF Vectorization** to convert text into numerical features
- Performed **train-test split** (75% training, 25% testing)

---

## 🤖 Models Used

Four supervised learning models were trained and evaluated:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **Gradient Boosting Classifier**

Each model was evaluated using:
- Accuracy Score
- Precision, Recall, F1-score
- Manual testing with real input text

---

## 🏆 Model Performance

| Model                   | Accuracy |
|------------------------|----------|
| Logistic Regression     | 98.41%   |
| Decision Tree           | 99.49%   |
| Random Forest           | 98.99%   |
| Gradient Boosting       | **99.59%** ✅ |

---

## 🧪 Manual Testing Function

A custom `manual_testing(news)` function was implemented that:
- Accepts a news paragraph as input
- Preprocesses and vectorizes it
- Runs predictions using all 4 models
- Prints whether the news is **"Fake"** or **"Not a Fake News"** per model

---

## 📂 Files Included

- <a href="Fake_&_True_News_Data">Click Here</a> – Datasets used 
- <a href="">Click Here</a> – Report and project summary  
- `README.md` – Project documentation

---

## 📈 Conclusion
This project demonstrates the ability of machine learning models to accurately classify fake vs. real news using simple text-based features and well-structured preprocessing. The results show strong performance, particularly with ensemble models like Gradient Boosting and Random Forest.
