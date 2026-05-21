# ECG Arrhythmia Classification Using Hybrid Deep Learning

## Project Overview
This project presents a hybrid deep learning architecture for ECG arrhythmia classification using multiple neural network components integrated into a unified pipeline.

The model combines:
- Convolutional Neural Networks (CNN)
- Gated Recurrent Units (GRU)
- Attention Mechanism
- Autoencoder (AE)

The objective of the project is to improve ECG heartbeat classification performance while demonstrating the integration of multiple deep learning blocks.

---

## Dataset
Dataset Used:
MIT-BIH Arrhythmia Dataset

Source:
PhysioNet

Dataset Characteristics:
- Original Samples: 87,554
- Working Subset: 3,000
- Features per Sample: 187
- Train/Test Split: 80/20

---

## Project Architecture

The proposed hybrid architecture includes:

### 1. CNN Block
Used for extracting local spatial ECG features.

### 2. GRU Block
Used for learning temporal dependencies in sequential ECG signals.

### 3. Attention Mechanism
Used to focus on important ECG regions and improve feature importance learning.

### 4. Autoencoder
Used for compressed latent feature representation and signal reconstruction.

---

## Data Preprocessing
The preprocessing pipeline includes:
- Feature and label separation
- Train/test splitting
- Data reshaping
- Feature normalization

---

## Training Process
The model was trained using:
- TensorFlow / Keras
- Adam optimizer
- Epoch-based training
- Validation monitoring

---

## Ablation Study
A systematic ablation study was conducted to evaluate the contribution of each architectural component.

Models evaluated:
- CNN Only
- CNN + GRU
- CNN + GRU + Attention
- AE + CNN + GRU + Attention

---

## Results
The hybrid model achieved stable ECG classification performance and demonstrated successful integration of multiple deep learning components.

The project also demonstrated:
- Effective feature extraction
- Sequential learning capability
- Improved representation learning
- Stable convergence during training

---

## Technologies Used
- Python
- TensorFlow
- Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib

---

## Authors
Deep Learning with Python Project