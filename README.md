# Email-Spam-Detection



## 📌 Overview
The **Email Classification Project** is a Machine Learning based application that automatically classifies emails into different categories such as:

- Spam
- Ham (Not Spam)
- Promotions
- Social
- Important
- Updates

This project helps in filtering emails intelligently, reducing manual effort, and improving email management efficiency.

---

## 🚀 Features
✅ Automatic email classification  
✅ Spam detection  
✅ Text preprocessing (cleaning + tokenization)  
✅ Feature extraction using NLP techniques  
✅ Machine Learning model training  
✅ Prediction on new emails  
✅ User-friendly interface (if web app added)  
✅ Fast and accurate results  

---

## 🛠️ Tech Stack

### Programming Language
- Python

### Libraries Used
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Matplotlib
- Seaborn
- Flask / FastAPI (if deployed)
- Pickle / Joblib

### Machine Learning Algorithms
- Naive Bayes
- Logistic Regression
- Random Forest
- SVM (optional)

---

## 📂 Project Structure

```bash
Email-Classification/
│
├── dataset/
│   └── emails.csv
│
├── models/
│   └── model.pkl
│
├── notebooks/
│   └── training.ipynb
│
├── app.py
├── preprocess.py
├── train_model.py
├── predict.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Working Process

### 1. Data Collection
Dataset contains email text and corresponding labels.

Example:

| Email | Label |
|------|------|
| Win ₹10,000 now | Spam |
| Meeting at 5 PM | Important |
| Big discount sale | Promotions |

---

### 2. Data Preprocessing
Cleaning text by:

- Lowercasing
- Removing punctuation
- Removing stopwords
- Tokenization
- Stemming / Lemmatization

Example:

Before:
```text
Congratulations!! You won cash prize.
```

After:
```text
congratul won cash prize
```

---

### 3. Feature Extraction
Convert text into numbers using:

- CountVectorizer
- TF-IDF Vectorizer

---

### 4. Model Training
Train model using classification algorithms.

Example:

```python
from sklearn.naive_bayes import MultinomialNB

model = MultinomialNB()
model.fit(X_train, y_train)
```

---

### 5. Prediction
Model predicts category of new email.

Example:

Input:
```text
Get 70% discount on shopping today.
```

Output:
```text
Promotions
```

---

## 📊 Model Performance
Metrics used:

- Accuracy
- Precision
- Recall
- F1-score

Example Results:

| Model | Accuracy |
|------|----------|
| Naive Bayes | 95% |
| Logistic Regression | 96% |
| Random Forest | 97% |

---

## ▶️ Installation

Clone repository:

```bash
git clone https://github.com/yourusername/email-classification.git
```

Move into folder:

```bash
cd email-classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run project:

```bash
python app.py
```

---

## 💻 Example Usage

```python
email = "Congratulations! You won a free iPhone."

prediction = model.predict([email])

print(prediction)
```

Output:

```text
Spam
```

---

## 🌟 Future Improvements
- Deep Learning model (LSTM / BERT)
- Multi-label classification
- Real-time email integration
- Dashboard analytics
- API deployment
- Cloud deployment

---

## 📸 Project Demo
(Add screenshots here)

- Home Page
- Prediction Page
- Results Page

---

## 🤝 Contribution
Contributions are welcome.

Fork repository → Create branch → Commit changes → Push → Pull Request

---

## 📜 License
This project is open-source under the MIT License.

---

## 👨‍💻 Author
**Shubham Jangra**  
Machine Learning Developer  
Python | ML | FastAPI | Data Science
