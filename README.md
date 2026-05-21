# ECG Arrhythmia Classification Using Hybrid Deep Learning

## Abstract
Electrocardiogram (ECG) analysis plays an important role in detecting cardiac arrhythmias and supporting clinical diagnosis. In this project, a hybrid deep learning architecture was developed for ECG arrhythmia classification using multiple neural network components integrated into a unified pipeline. The proposed model combines Convolutional Neural Networks (CNN), Gated Recurrent Units (GRU), Attention Mechanism, and Autoencoder (AE) blocks to improve feature extraction and sequential pattern learning from ECG heartbeat signals.

---

# 1. Introduction

Deep learning techniques have recently shown strong performance in healthcare applications, especially in biomedical signal analysis. ECG signals contain complex temporal patterns that require robust feature extraction and sequential learning capabilities.

Traditional machine learning methods often require manual feature engineering, while deep learning models can automatically learn representations directly from raw ECG signals.

This project aims to develop a hybrid deep learning architecture capable of improving ECG arrhythmia classification performance through integrated multi-block learning.

---

# 2. Dataset

Dataset Used:
MIT-BIH Arrhythmia Dataset

Source:
PhysioNet

Dataset Characteristics:
- Original Samples: 87,554
- Working Subset: 3,000
- Features per Sample: 187
- Train/Test Split: 80/20

The dataset contains ECG heartbeat signals collected from multiple patients and annotated for arrhythmia classification research.

---

# 3. Data Preprocessing

The preprocessing pipeline includes several steps before training:

1. Feature and label separation
2. Train/test split
3. Data reshaping
4. Feature normalization

The ECG signals were reshaped into formats compatible with convolutional and recurrent neural network layers.

---

# 4. Proposed Hybrid Architecture

The proposed architecture integrates four major components:

## 4.1 CNN Block
The CNN block extracts local spatial features from ECG heartbeat windows using convolutional filters.

## 4.2 GRU Block
The GRU block learns temporal dependencies and sequential ECG patterns.

## 4.3 Attention Mechanism
The attention layer helps the model focus on important ECG regions and informative signal segments.

## 4.4 Autoencoder Block
The autoencoder compresses ECG signals into compact latent representations and reconstructs them to improve feature learning.

---

# 5. Training Process

The model was implemented using TensorFlow and Keras.

Training configuration:
- Optimizer: Adam
- Loss Functions: MSE and categorical classification loss
- Epochs: 3
- Batch Size: 32

Validation monitoring was used to observe convergence behavior during training.

---

# 6. Ablation Study

A systematic ablation study was conducted to evaluate the contribution of each model component.

The following architectures were tested:
- CNN Only
- CNN + GRU
- CNN + GRU + Attention
- AE + CNN + GRU + Attention

The ablation study demonstrated how integrated hybrid learning affects ECG classification performance.

---

# 7. Results

The proposed hybrid model achieved stable ECG classification performance and demonstrated successful integration of multiple deep learning components.

Key outcomes:
- Effective feature extraction
- Sequential dependency learning
- Improved latent representation learning
- Stable training convergence

---

# 8. Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

# 9. Conclusion

This project successfully developed a hybrid ECG arrhythmia classification model combining CNN, GRU, Attention, and Autoencoder components.

The results demonstrate that hybrid deep learning architectures can effectively analyze biomedical signals and support automated healthcare applications.

Future improvements may include:
- Larger datasets
- Transformer-based architectures
- Hyperparameter optimization
- Real-time deployment systems