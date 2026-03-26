# EEG-Schizophrenia-CNN-BiLSTM
Hybrid 1D CNN–BiLSTM model for EEG-based schizophrenia classification

This repository presents a lightweight hybrid deep learning model for automated schizophrenia (Scz) detection using EEG signals. The proposed framework integrates:

1D Convolutional Neural Networks (CNN) → spatial feature extraction
Bidirectional Long Short-Term Memory (Bi-LSTM) → temporal dependency learning

The model is designed to be computationally efficient, accurate, and suitable for real-time clinical applications.

🎯 Key Contributions
✅ Novel CNN + Bi-LSTM hybrid architecture for EEG classification
✅ Eliminates need for manual feature engineering
✅ Works with raw EEG signals (no heavy preprocessing required)
✅ Evaluated on two public EEG datasets
✅ Lightweight model (~0.76M parameters) suitable for deployment
✅ Frequency-band level analysis (Delta, Theta, Alpha, Beta, Gamma)
🧪 Datasets

This study uses two publicly available EEG datasets:

1️⃣ Moscow Dataset
84 subjects (39 HC, 45 Scz)
16-channel EEG
Sampling rate: 128 Hz
Duration: 60 seconds

🔗 http://brain.bio.msu.ru/eeg_SZ.htm

2️⃣ IBIB PAN Dataset
28 subjects (14 HC, 14 Scz)
19-channel EEG
Sampling rate: 250 Hz
Duration: 15 minutes

🔗 https://repod.icm.edu.pl/dataset.xhtml?persistentId=doi:10.18150/repod.0107441

⚙️ Methodology

The proposed pipeline consists of:

Preprocessing
Z-score normalization
PCA (only for IBIB PAN dataset)
Model Architecture
1D CNN layers → extract local spatial features
Bi-LSTM layers → capture temporal dependencies
Fully connected layers → classification
Training
Optimizer: Adam
Loss: Binary Cross-Entropy
Epochs: 100
Batch size: 32
🏗️ Model Architecture
Input EEG → CNN Layers → Feature Maps → Bi-LSTM → Dense Layers → Output
CNN captures waveform patterns
Bi-LSTM captures temporal dynamics
Output: Binary classification (HC vs Scz)

## 👩‍💻 Author
Anjali Sagar Jangde
