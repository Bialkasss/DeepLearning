# 🔍 Anomaly Detection in Time Series Classification


## 🎯 Project Goal

The objective is to:
- ✅ Correctly classify multivariate time series into their respective classes  
- 🔍 Highlight **which part** of the signal is responsible for the defect/anomaly  
- 🧠 Use **neural networks with recurrent layers** to capture temporal patterns  
- 🔁 Design an approach that generalizes to other datasets after retraining

> This project goes further — into **interpretable detection** and **explanation**.

---

## 🛠️ How It Was Done

### 1. Data Generation 📈  
Synthetic time series were generated, each class following a distinct pattern with occasional anomalies.

### 2. Preprocessing 🔧  
- Time series were normalized and padded to a consistent shape  
- Data was split into train/validation/test sets  
- Used `MinMaxScaler` and custom data loaders

### 3. Model Architecture 🧠  
- Built a **deep neural network** with:
  - `LSTM` layers for temporal understanding
  - `Conv1D` layers to detect local patterns
  - `Dense` layers for classification
  - Masking and attention-inspired components for interpretability

### 4. Training & Evaluation 🧪  
- Trained on synthetic data  
- Evaluated using accuracy, precision, recall  
- Highlighted time steps contributing to the classification decision (for defect explainability)  

---

## 💻 Technologies Used

- Python 🐍  
- TensorFlow / Keras 🔁  
- NumPy & Pandas 📊  
- Matplotlib for visualizations 📉  
- Scikit-learn for metrics and preprocessing  

---

## 📸 Visuals

| Predicted Class | Explanation Highlight |
|-----------------|------------------------|
| Class 1, 3 ✅ | ![highlight](https://github.com/Bialkasss/DeepLearning/blob/f406c348536a8532d494b38c018b9fe21415d1ea/RNN/Candies/Screenshot_1.png) |
| Class 1, 3 ✅ | ![highlight](https://github.com/Bialkasss/DeepLearning/blob/f406c348536a8532d494b38c018b9fe21415d1ea/RNN/Candies/anomalies.png) |

---

## Author
Maria Musiał

- Improve generalization to real-world sensor datasets  
- Extend to multivariate/multi-label settings  
- Integrate more advanced interpretability methods (e.g., SHAP, attention heatmaps)  

---

Let me know if you'd like this in Polish 🇵🇱, want to embed output plots directly, or need help generating a nice cover image.
