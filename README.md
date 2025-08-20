# ATTENTION-GUIDED-MULTISCALE-CNN-USING-EEG-SIGNALS-FOR-DRIVER-DROWSINESS-DETECTION
 ## NeuroAlert: EEG-Based Driver Drowsiness Detection Using Deep Learning

> ⚡ A deep learning pipeline to detect driver drowsiness from EEG signals using advanced CNN architectures, wavelet transforms, and attention mechanisms.

### 🧠 Project Overview

Driver drowsiness is a leading cause of road accidents globally. To address this issue, our project leverages EEG signals to classify alert vs. drowsy brain states using a series of novel deep learning models.

We used **SEED-VIG EEG dataset** and designed multiple deep learning architectures combining:
- Continuous Wavelet Transform (CWT)
- Multiscale CNNs
- EEG-ATCNet
- Attention Mechanisms: CBAM, SE-Attention

Each model enhances EEG feature extraction, attention to critical signal regions, and performance reliability through validation techniques like **K-Fold Cross-Validation**.


---

## 🧪 Dataset Details

- **Dataset:** `SEED_VIG_processed.csv`
- **Channels:** 17 EEG channels
- **Samples:** 12 subjects in driving simulator
- **Timepoints:** 384 per channel
- **Labels:** 
  - `0` = Alert (Normal)
  - `1` = Drowsy (Fatigued)
- **Total Features:** 6,528 EEG features + 2 identifiers = 6,530 columns

---

## 📊 Models and Performance Summary

| Model Configuration                                     | Accuracy | F1-Score | Recall | Precision |
|---------------------------------------------------------|----------|----------|--------|-----------|
| EEG-ATCNet                                              | 94.2%    | 0.94     | 0.94   | 0.95      |
| Multiscale CNN + CBAM                                   | 97.05%   | 0.97     | 0.97   | 0.97      |
| Multiscale CNN + CBAM + K-Fold                          | 96.28%   | 0.96     | 0.96   | 0.96      |
| Multiscale CNN + SE Attention                           | 96.5%    | 0.97     | 0.95   | 0.98      |

---

## ⚙️ Key Techniques Used

- **CWT (Continuous Wavelet Transform)**: For converting raw EEG signals to time-frequency representations
- **Multiscale CNN**: For feature extraction at multiple temporal resolutions
- **EEG-ATCNet**: Temporal convolutional layers tailored for EEG data
- **Attention Mechanisms**:
  - **CBAM** (Convolutional Block Attention Module)
  - **SE-Attention** (Squeeze-and-Excitation)
  - **ICNN** (Improved Channel-wise Nonlinear Attention)
- **K-Fold Cross-Validation**: To ensure generalization across EEG samples



