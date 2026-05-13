**EEG Eye State Anomaly Detection using Deep Learning**

**Overview**

This project presents an EEG-based eye state detection system using anomaly detection and deep learning techniques. The system analyzes brain signals to classify eye states (open/closed) and detect abnormal patterns in real-time.

The study compares four approaches:

\- One-Class Support Vector Machine (OCSVM)

\- Isolation Forest (IF)

\- Autoencoder (AE)

\- Proposed Temporal Stacked Autoencoder (TSAE)

The proposed TSAE model achieves superior performance by capturing temporal dependencies in EEG signals.

---

**Objectives**

\- Preprocess EEG signals for reliable analysis

\- Detect anomalies in EEG eye state data

\- Compare multiple anomaly detection techniques

\- Develop a temporal deep learning model (TSAE)

\- Minimize false alarms in real-time detection

---

**About EEG**

Electroencephalography (EEG) records electrical activity of the brain using electrodes placed on the scalp. It is:

\- Non-invasive

\- High temporal resolution

\- Widely used in medical and research applications

---

**Dataset**

\- \*\*Name:\*\* EEG Eye State Dataset

\- \*\*Source:\*\* UCI Machine Learning Repository

\- \*\*Samples:\*\* 14,980

\- \*\*Features:\*\* 14 EEG channels \+ 1 label

\- \*\*Sampling Rate:\*\* 128 Hz

\#\#\# Target:

\- `0` → Eyes Open

\- `1` → Eyes Closed

---

\#\# System Architecture

1\. \*\*Signal Acquisition\*\*

   \- EEG signals collected from 14 channels

2\. \*\*Preprocessing\*\*

   \- Bandpass filtering (0.5–45 Hz)

   \- Artifact removal (ICA)

   \- Normalization (Z-score)

3\. \*\*Feature Extraction\*\*

   \- Power Spectral Density (PSD)

   \- Wavelet features

   \- Time-frequency analysis

4\. \*\*Learning Models\*\*

   \- OCSVM (boundary-based)

   \- Isolation Forest (isolation-based)

   \- Autoencoder (reconstruction-based)

   \- TSAE (temporal deep learning)

5\. \*\*Output\*\*

   \- Eye State Prediction (Open / Closed)

---

\#\# Technologies Used

\- Python

\- NumPy, Pandas

\- Scikit-learn

\- TensorFlow / PyTorch

\- Signal Processing Techniques

---

\#\#  Models Implemented

\#\#\# 1\. OCSVM

\- Learns boundary of normal EEG data

\- Detects deviations as anomalies

\#\#\# 2\. Isolation Forest

\- Isolates anomalies using random trees

\- Efficient for large datasets

\#\#\# 3\. Autoencoder

\- Learns reconstruction of normal signals

\- High reconstruction error → anomaly

\#\#\# 4\. TSAE (Proposed Model)

\- Stacked deep autoencoder

\- Captures temporal dependencies

\- Best performance among all models

---

\#\#  Performance Metrics

\- Accuracy

\- Precision

\- Recall

\- F1-Score

\- ROC-AUC

\- PR-AUC

\- False Alarm Rate (FAR)

\- Event Detection Rate (EDR)

---

\#\# Results Summary

| Model   | ROC-AUC | PR-AUC | Recall @ FAR=1% |

|--------|--------|--------|----------------|

| OCSVM  | 0.7667 | 0.8306 | 0.3333 |

| IF     | 0.8667 | 0.8972 | 0.5000 |

| AE     | 0.9667 | 0.9762 | 0.8333 |

| TSAE   | \*\*1.0000\*\* | \*\*1.0000\*\* | \*\*1.0000\*\* |

 \*\*TSAE achieved the best performance with perfect detection accuracy and zero false alarms.\*\*

---

\#\#  Computational Efficiency

| Model | Inference Time (ms) |

|------|------------------|

| OCSVM | 0.52 |

| IF | 26.37 |

| AE | 56.73 |

| TSAE | 71.37 |

\- OCSVM → Fastest

\- TSAE → Most accurate

---

\#\#  How to Run the Project  
1\. Open Google browser and search for google colab   
2\. Create a new notebook in google colab   
3\. Copy the code from the source code for each model and paste in the notebook   
4\. Enter shift+ enter to run    
5\. Upload the dataset file  
6\. observe the graphs and plots 6\. Repeat this process for every model.

