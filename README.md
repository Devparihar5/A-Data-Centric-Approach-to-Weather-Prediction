# A Data-Centric Approach to Weather Prediction: IoT and Machine Learning on Drone Platforms

### IoT and Machine Learning on Drone Platforms

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PDF](https://img.shields.io/badge/Read--Paper-InGARSS--2024-orange)](./InGARSS-24.pdf)

## 📄 Abstract

This research presents a **drone-based weather prediction system** that leverages **IoT sensor networks and machine learning algorithms** to optimize agricultural decision-making. The approach combines **real-time sensing**, **edge computing**, and **pre-trained ML/DL models** to achieve high-accuracy weather forecasts in remote agricultural areas, minimizing latency and enhancing responsiveness.

---

## 🔍 Problem Statement

Modern agriculture demands precise environmental monitoring. However, **low-cost IoT devices** often lack the computational capabilities required for real-time predictions using traditional machine learning techniques. Cloud computing introduces latency, making timely actuation difficult in critical scenarios like rainfall or frost warnings.

---

## 🚁 Proposed Solution

We propose a **hybrid edge-cloud framework** where:

* Historical weather data is used to **train ML/DL models** (Logistic Regression, XGBoost, CatBoost, etc.).
* These models are **deployed on edge nodes mounted on drones** to reduce latency.
* **IoT sensors** capture real-time environmental data which is processed onboard by the drone.
* The system provides **real-time actuation decisions** for agricultural automation (e.g., irrigation, pesticide spraying).

---

## 🧠 Machine Learning Models Evaluated

| Model               | Performance (Australia Dataset) | Performance (Bikaner Dataset) |
| ------------------- | ------------------------------- | ----------------------------- |
| Logistic Regression | 79.5% Accuracy                  | **91.3% Accuracy**            |
| Decision Tree       | 86.1% Accuracy                  | 88.3% Accuracy                |
| Random Forest       | 92.7% Accuracy                  | 90.8% Accuracy                |
| **XGBoost**         | **94.96% Accuracy**             | 90.3% Accuracy                |
| CatBoost            | 93.9% Accuracy                  | 91.2% Accuracy                |
| LightGBM            | 86.6% Accuracy                  | 90.8% Accuracy                |

📈 Evaluation Metrics: Accuracy, Precision, Recall, F1-score, Cohen’s Kappa, AUC-ROC.

---

## 🌍 Datasets Used

* **Rain in Australia** ([Kaggle](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package))
* **Bikaner (India) Weather Data**: Collected from [NASA POWER Project](https://power.larc.nasa.gov/) and [IMDLib](https://pypi.org/project/imdlib/)

---

## ⚙️ System Architecture

1. **Cloud Layer**: Train models on historical weather data.
2. **Edge Layer (Drone)**: Deploy pre-trained model for real-time inference.
3. **IoT Layer**: Sensors collect temperature, humidity, pressure, etc.
4. **Actuator Layer**: Executes automated decisions on the field.

---

## 🔬 Experimental Results

* **XGBoost** achieved the **highest prediction accuracy (94.96%)** on the Australian dataset.
* **Logistic Regression** performed best on the **Bikaner dataset**.
* **Drone-mounted edge nodes** demonstrated real-time capability with low-latency decision-making.

---

## 🧾 Citation

If you find this research helpful, please consider citing:

```bibtex
@INPROCEEDINGS{10984355,
  author={Parihar, Devendra and Chaudhary, Ajay and Peddoju, Shreehitha and Kadarla, Kavitha},
  booktitle={2024 IEEE India Geoscience and Remote Sensing Symposium (InGARSS)}, 
  title={A Data-Centric Approach to Weather Prediction: IoT and Machine Learning on Drone Platforms}, 
  year={2024},
  volume={},
  number={},
  pages={1-4},
  keywords={Machine learning algorithms;Accuracy;Computational modeling;Decision making;Weather forecasting;Machine learning;Prediction algorithms;Sensors;Internet of Things;Drones;Internet of Things;IoT;Edge Node;Drone;Weahter Predition;Weather Forecasting;Precision Farming;Smart Agriculture;Machine Learning},
  doi={10.1109/InGARSS61818.2024.10984355}}
```

---

## 🤝 Contributions & Acknowledgements

* **Devendra Parihar** – AI Developer at Helios Solutions, Vadodara, India
* **Ajay Chaudhary** – Engineering College Bikaner, India
* **Shreehitha Peddoju** – NIT Rourkela
* **Kavitha Kadarla** – COER University, Roorkee

Special thanks to datasets from **NASA**, **IMD**, and **Kaggle**.

---

## 📬 Contact

For queries, reach out to:
📧 [devendraparihar340@gmail.com](mailto:devendraparihar340@gmail.com)
