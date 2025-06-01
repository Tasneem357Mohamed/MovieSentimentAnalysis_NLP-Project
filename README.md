
# 🎬 Sentiment Analysis of Movie Reviews

This project performs **sentiment analysis** on movie reviews using machine learning techniques. Reviews are classified as **positive** or **negative**, and the model's training process is visualized and evaluated.

---

## 📁 Dataset

We use the **Sentiment Polarity Dataset v1.0** from Cornell:
- Link: [Cornell Movie Review Data](https://www.cs.cornell.edu/people/pabo/movie-review-data/)
- It contains:
  - `pos/` folder: positive movie reviews
  - `neg/` folder: negative movie reviews

The dataset is split into:
- **Training Set** (for training the ML model)
- **Test Set** (for evaluating performance)

---

## ⚙️ Process Workflow

### 1. **Data Preprocessing**
- Reading all `.txt` files
- Removing punctuation, special characters
- Tokenization and stop word removal
- Lowercasing and normalization

### 2. **Feature Extraction**
- Used **TF-IDF Vectorization** to convert text data into numerical features.

### 3. **Model Training and Testing**
- Models Tried:
  - Logistic Regression
  - Naive Bayes
  - Support Vector Machine (SVM)
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

## 📊 Results

- **Best Model**: *(e.g., Logistic Regression)*
- **Accuracy**: *~XX%* on test set
- **Classification Report**:
  ```
  Precision  Recall  F1-score
  Pos:  0.XX     0.XX    0.XX
  Neg:  0.XX     0.XX    0.XX
  ```

- **Confusion Matrix**:
  ```
       Predicted
       Pos  Neg
  Pos [ TP   FN ]
  Neg [ FP   TN ]
  ```

---

## 🧪 How to Run

1. **Install Requirements**
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the Notebook**
   Open and run all cells in `Movie_Deployment.ipynb`

3. **Model Output**
   - Model performance is printed
   - Charts are generated for visualization
   - Best model is saved as `best_model.pkl`

---

## 📂 Project Structure

```
📁 dataset/
   ├── pos/
   └── neg/
📄 Movie_Deployment.ipynb
📄 README.md
📄 requirements.txt
```

---

## 💬 Notes

- Ensure the dataset folders are correctly named `pos` and `neg`.
- This notebook is intended for educational use and could be expanded with deep learning models or hyperparameter tuning.
