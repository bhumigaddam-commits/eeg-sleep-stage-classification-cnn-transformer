EEG Sleep Stage Classification using CNN-Transformer

A research-oriented deep learning framework for automated sleep stage classification using EEG signals from the Sleep-EDF (PhysioNet) dataset.

This project implements a hybrid CNN-Transformer architecture to capture both local temporal patterns and long-range temporal dependencies in EEG time-series data.


Project Overview

Sleep stage classification is a fundamental task in computational neuroscience and clinical sleep research. Manual scoring is time-consuming and subject to inter-rater variability, making automated solutions highly valuable.

This work proposes a hybrid deep learning model that:
- Extracts spatial-temporal features using Convolutional Neural Networks (CNN)
- Captures global temporal dependencies using Transformer Encoder layers
- Classifies EEG signals into multiple sleep stages


Dataset

Dataset used: Sleep-EDF Expanded (PhysioNet)  
Signal type: EEG  
Sleep stages: Wake (W), N1, N2, N3, REM  
Sampling frequency: 100 Hz  

Preprocessing steps:
- Signal normalization
- Segmentation into 30-second epochs
- Label encoding
- Train-validation-test split


Model Architecture

The model consists of three main components:

1. CNN-based feature extractor  
   - 1D Convolution layers  
   - Batch normalization  
   - ReLU activation  
   - Max pooling  

2. Transformer encoder  
   - Multi-head self-attention  
   - Positional encoding  
   - Feed-forward network  
   - Layer normalization  

3. Fully connected classification head  
   - Dropout regularization  
   - Softmax output layer  

This hybrid design allows the model to learn both short-term EEG patterns and long-range contextual relationships.


Evaluation Metrics

Model performance is evaluated using:
- Accuracy  
- ROC-AUC score  
- Confusion matrix  
- Precision, Recall, F1-score  
- False negative rate (critical in medical analysis)


Research Relevance

- Reduces dependency on manual sleep scoring  
- Demonstrates the applicability of Transformer models in EEG analysis  
- Bridges deep learning and computational neuroscience  
- Potential applications in sleep disorder detection (e.g.Obstructive Sleep Apnea)

Author

Bhumika Gaddam  
B.Tech CSBS | Data Science Minor (IIT Guwahati)  
AI & Computational Neuroscience Enthusiast
