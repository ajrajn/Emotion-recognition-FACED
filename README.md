# Emotion-recognition-FACED
EEG emotion classification project using frequency-domain features and Leave-One-Subject-Out validation to evaluate subject-independent machine learning performance.
EEG Emotion Recognition Using PSD and Differential Entropy Features

Project Overview

This project implements an EEG-based emotion recognition pipeline using frequency-domain features. The goal is to classify emotional states by analyzing neural activity patterns and evaluating subject-independent model performance.

Dataset and Labels

This project uses the FACED (Fine-grained Affective Computing EEG Dataset), a large-scale multi-subject EEG dataset designed for emotion recognition research.

FACED dataset characteristics:

- Number of subjects: 123  
- EEG channels: 32  
- Sampling rate: 250 Hz  
- Number of emotion categories: 9  
- Trials per subject: 28  
- Recording protocol: Emotion elicitation using video stimuli  

Emotional labels are mapped based on valence categories to enable supervised learning. Subject-wise organization is preserved to ensure realistic evaluation.

Methodology

The processing pipeline includes:

1. Loading pre-extracted EEG features  
2. Feature aggregation across trials and subjects  
3. Label mapping for emotion classes  
4. Data reshaping and normalization  
5. Subject-wise train-test splitting using Leave-One-Subject-Out (LOSO) validation  
6. Supervised classification and performance evaluation  

Validation Strategy

Leave-One-Subject-Out cross-validation is used to evaluate model generalization across unseen subjects. This approach reflects real-world EEG deployment scenarios where models must adapt to new users.

Tools and Libraries

- Python  
- NumPy  
- SciPy  
- Scikit-learn  
- Matplotlib  

How To Run

1. Open the notebook file  
2. Ensure FACED dataset paths are correctly set  
3. Run all cells sequentially to reproduce results  

Output

The notebook generates classification performance metrics for emotion recognition and evaluates cross-subject generalization capability.
