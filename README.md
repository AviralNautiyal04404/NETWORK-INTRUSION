Real-Time AI-Based Network Intrusion Detection System (NIDS)

This project implements a real-time, machine learning-based Network Intrusion Detection System using the NSL-KDD dataset and a trained Random Forest classifier. It monitors live network traffic and classifies each packet as **normal** or **intrusion**, raising alerts accordingly.

---

## 📌 Features

- ✅ Real-time network packet sniffing
- ✅ Feature extraction modeled after NSL-KDD dataset
- ✅ Pre-trained Random Forest intrusion classifier
- ✅ Alert generation and logging
- ✅ Modular and scalable Python project
- ✅ Ready for integration with GUI or dashboards
- ✅ Performance evaluation tools included

---

## 📁 Project Structure
real_time_nids_project/
├── model/
│ └── nids_rf_model.joblib # Trained Random Forest model
├── core/
│ ├── feature_extraction.py # Extracts features from packets
│ ├── packet_sniffer.py # Captures and classifies packets
│ └── utils.py # Label encoders and helpers
├── logs/
│ └── alerts.log # Intrusion alerts log
├── main.py # Main entry point
├── requirements.txt # Dependencies
└── README.md

## 🧪 Prerequisites

Make sure Python is installed (`>=3.7`), then install dependencies:

```bash
pip install -r requirements.txt
This project uses:
scapy for packet capture
pandas, joblib, and scikit-learn for ML

TO RUN :- sudo python3 main.py

Model Type: Random Forest Classifier
Training Dataset: NSL-KDD
Input Features: 41 features (matching NSL-KDD structure)

Performance evaluation scripts are included to display:

Accuracy
Precision, Recall, F1-Score
Confusion Matrix
t-SNE Plot (2D visualization)
Outlier Detection & Robustness Testing

Known Limitations

Only a subset of NSL-KDD features are extractable in live traffic
Real-time feature engineering is simplified
Some fields are mocked or zero-filled (e.g., duration, land, etc.)

 Future Enhancements

GUI dashboard using Tkinter or Streamlit
Deep learning models with Keras
Docker container for easy deployment
Automatic periodic model retraining
REST API to expose alerts

