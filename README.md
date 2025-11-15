# 📰 Fake News Detection — Machine Learning Project

## Overview  
This project builds a **Fake News Detector** using Natural Language Processing (NLP) and machine learning. The system classifies news headlines as **real** or **fake** based on a dataset of labeled news items.

## Dataset  
- **Source:** `FakeNewsNet.csv`  
- **Location used in code:** `/home/junaid/Downloads/FakeNewsNet.csv` (or you can move it to `data/raw/`)  
- **Key columns used:**
  - `title` — the news headline / text  
  - `real` — binary label (1 = real, 0 = fake)  

## Pipeline / Architecture  

1. **Data Loading**  
   - Load CSV using a data loader script  
2. **Preprocessing**  
   - Clean text: lowercase, remove URLs and non-letter characters  
   - Prepare training and test split  
3. **Feature Engineering**  
   - TF-IDF vectorization (1-2 grams)  
4. **Model Training**  
   - Trained four different classifiers:
     - Logistic Regression  
     - Multinomial Naive Bayes  
     - Passive Aggressive Classifier  
     - Linear SVC  
   - Select the “best” model based on test accuracy  
5. **Evaluation**  
   - Generate classification report (precision, recall, F1-score)  
   - Plot and save a confusion matrix  
6. **Prediction / Inference**  
   - Provide a function / simple script to predict a new headline  
7. **(Optional) Extendability**  
   - LSTM-based deep learning baseline (if TensorFlow is installed)  
   - (Template for) BERT-based model fine-tuning  

## Results  
- Best model: *Passive Aggressive* / *Logistic Regression* (or your chosen best)  
- Accuracy: ~**`<your-accuracy>`** (replace with your actual result)  
- Confusion matrix saved as `outputs/confusion_matrix.png`  
- Classification report saved in `outputs/classification_report.txt`

 
