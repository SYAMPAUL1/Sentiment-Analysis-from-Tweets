# 📝 Sentiment Analysis from Tweets  

---

## 📌 Project Overview

This assignment involved building a **text classification pipeline** to analyze **sentiment in tweets**, using a dataset of approximately 27,000 labelled entries. The task was to predict whether a given tweet expresses a **REAL** or **FAKE** sentiment.

The workflow included:
- Preprocessing and tokenization
- Feature extraction
- Classifier training with SVM
- Cross-validation and model evaluation
- Error analysis using confusion matrices and performance metrics

---

## 📂 Dataset

- Format: TSV (Tab-Separated Values)
- Approx. 27,000 rows
- Labels: `REAL` or `FAKE`
- Split: 80% training, 20% testing

---

## ⚙️ Functionality

### 1. **Preprocessing**
- Regex-based punctuation separation
- Whitespace tokenization
- Case normalization (lowercasing)
- [Optimized version includes stopword removal, lemmatization]

### 2. **Feature Extraction**
- Token frequency vectors using dictionaries
- Global token tracking with `global_feature_dict`

### 3. **Training**
- Linear Support Vector Classifier (`LinearSVC`)
- Sklearn pipeline for streamlined training

### 4. **Cross-Validation**
- Custom `cross_validate()` function with configurable k-fold logic
- Performance metrics: **Precision**, **Recall**, **F1-score**, **Accuracy**

### 5. **Error Analysis**
- Confusion matrix heatmap visualization
- Identification and printing of false positives/negatives

---

## 📊 Performance Metrics (10-fold Cross-Validation)

| Metric     | Value (avg) |
|------------|-------------|
| Precision  | ~**X.XX**   |
| Recall     | ~**X.XX**   |
| F1-Score   | ~**X.XX**   |
| Accuracy   | ~**X.XX**   |

*(Replace X.XX with your actual numbers if known.)*

---

## 🛠️ Technologies Used

- Python 3  
- scikit-learn  
- NLTK  
- NumPy  
- Matplotlib  
- Custom SVM pipeline and data handling functions

---

## 🧪 How to Run

1. Clone the repository  
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
