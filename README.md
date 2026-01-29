# 🚀 Edge AI for Real-Time Video Anomaly Detection

## 📌 Project Overview
This project implements an **unsupervised CNN–LSTM Autoencoder** to detect anomalous
activities in video streams. The model is trained **only on normal videos** and
identifies anomalies using **reconstruction error thresholding**.

The system is optimized for **edge deployment** and does not require labeled anomaly data.

---

## 🎯 Key Features
- Unsupervised anomaly detection
- CNN for spatial feature extraction
- LSTM for temporal modeling
- Reconstruction error–based anomaly scoring
- CPU-friendly (Google Colab compatible)
- Edge-ready (TFLite export supported)

---

## 📊 Dataset
**UCSD Pedestrian Dataset**
- Training: Normal pedestrian walking videos
- Testing: Normal + anomalous activities (bikes, carts, vehicles)

> Dataset is automatically downloaded inside the notebook and is **not included**
> in this repository.

---

## 🧠 Model Architecture
- **Encoder**: CNN + LSTM
- **Decoder**: LSTM + CNN
- **Loss Function**: Mean Squared Error (MSE)
- **Detection Method**: Reconstruction error threshold

---

## 📈 Results
- Recall (Anomaly Detection Rate): ~27%
- Precision: ~44%
- Threshold-based detection
- Conservative detection with low false alarms

> Moderate recall is expected due to subtle anomalies in UCSD dataset.

---

## ⚙️ How to Run
1. Open the notebook in **Google Colab**
2. Run all cells from top to bottom
3. Dataset will be downloaded automatically
4. Model trains using normal videos only
5. Anomalies are detected during testing

---

## 🛠️ Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Scikit-learn

---

## 💡 Why Autoencoder?
- No need for labeled anomaly data
- Can detect unseen anomaly types
- Suitable for real-world surveillance
- Handles class imbalance naturally

---

## 📌 Author
Mohamed Tahir

