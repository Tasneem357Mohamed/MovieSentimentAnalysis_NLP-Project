# 🎬 Sentiment Analysis of Movie Reviews

This project performs **sentiment analysis** on movie reviews using machine learning techniques. Reviews are classified as **positive** or **negative**, and the model's training process is visualized and evaluated.

---
## Table Of Content
- [Deployement Website](#deployement-website)
- [Dataset](#dataset)
- [Process Workflow](#process-workflow)
- [Results](#results)
- [Notes](#notes)
- [Contributors](#contributors)


---
## Deployement Website
![WhatsApp Image 2025-05-23 at 03 25 58](https://github.com/user-attachments/assets/4972ca86-6c4c-4c5a-9279-d85bcb64c0cf)

---
## Dataset

We use the **Sentiment Polarity Dataset v1.0** from Cornell:
- Link: [Cornell Movie Review Data](https://www.cs.cornell.edu/people/pabo/movie-review-data/)
- It contains:
  - `pos/` folder: positive movie reviews
  - `neg/` folder: negative movie reviews

The dataset is split into:
- **Training Set** (for training the ML model)
- **Test Set** (for evaluating performance)

---

## Process Workflow

### 1. **Data Preprocessing**
- Reading all `.txt` files
- Removing Duplicates and Stopwords
- Removing punctuation, special characters
- Tokenization and stop word removal
- Lowercasing and normalization

### 2. **Feature Extraction**
- Used **TF-IDF Vectorization** to convert text data into numerical features.

### 3. **Model Training and Testing**
- ML Models:
  - Logistic Regression
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Random Forest
  - KNN
  - Decision Tree
- ML Models:
  - LSTM
  - RNN
  - GRU
- Dataset split: 80% training / 20% testing
- Performance metrics:
  - Accuracy
  - Confusion Matrix
  - Classification Report

### 4. **Visualizing Results**
- Accuracy comparison bar chart
- Confusion matrix heatmap
- Model training performance curve (if applicable)

### 5. **Saving the Best Model**
- The best-performing model is saved using `joblib` or `pickle`.

---

## Results
### Best Model --> ML Model (SVM Model: with Kernel => Linear)
### * Best Parameters: {'C': 1}
### * Best CV F1-Score: 89.49%
### * Train Accuracy: 95.875%
### * Test Accuracy: 87.75%
<img width="928" alt="Screenshot 2025-06-01 at 3 45 36 AM" src="https://github.com/user-attachments/assets/33980952-c978-4a23-ae0a-f31a56a4e328" />

---

## Notes

- Ensure the dataset folders are correctly named `pos` and `neg`.
- This notebook is intended for educational use and could be expanded with deep learning models or hyperparameter tuning.

---
## Contributors
|                   Name                    |     Github Link    |
| :---------------------------------------: | :--------: |
|      Tasneem Mohamed Ahmed Mohamed     | https://github.com/Tasneem357Mohamed |
| Bsmala Tarek Kamal Khalil Elbagoury | https://github.com/Bsmalatarek |
|     Nora Ahmed Salem Ahmed   | https://github.com/Nora-Ahmed |
|          Amira Mostafa Haroon Abde/Wahaab          | https://github.com/amira468 |
|           Shahd Sherif Wagdy Khalifa          | https://github.com/shahdsherif29 |
|       Mennatullah Alaa Ahmed        |  |
