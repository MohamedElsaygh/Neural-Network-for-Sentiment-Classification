# 🧠 Task 3: Neural Network for Sentiment Classification

This task involves training a neural network to classify social media posts into sentiment categories using TensorFlow and Keras.

---

## 📌 Objective

- Build and train an LSTM-based sentiment classifier  
- Handle imbalanced classes using class weighting  
- Evaluate model performance and analyze metrics  

---

## 📁 Dataset

- Input: `Text` column from the CSV file  
- Output: `Sentiment` (top 5 most frequent classes kept)  
- Preprocessing:  
  - Tokenization  
  - Padding sequences  
  - Label encoding

---

## 🏗️ Model Architecture

- `Embedding` layer  
- `LSTM` layer  
- `Dropout` layers for regularization  
- `Dense` output layer with `softmax` activation

---

## ⚙️ Training Details

- Loss: `categorical_crossentropy`  
- Optimizer: `Adam`  
- Epochs: 20  
- Batch size: 32  
- EarlyStopping used to prevent overfitting  
- Class weights applied to address imbalance

---

## 📊 Evaluation

- Accuracy: ~63% on test set  
- Best performance on the majority class (`Positive`)  
- Struggles with underrepresented classes  
- Evaluation metrics: precision, recall, F1-score, confusion matrix

---

## 🧾 Summary

The model captures sentiment patterns well for common classes but shows poor generalization for rare ones.  
Future improvements could include:  
- Pre-trained embeddings (GloVe, BERT)  
- Data augmentation  
- Attention mechanisms  

---

## ✅ Status

✔️ Task Completed  
🧪 Tested on real validation/test data  
📂 Notebook: `Task_3_Neural_Network_for_Sentiment.ipynb`
