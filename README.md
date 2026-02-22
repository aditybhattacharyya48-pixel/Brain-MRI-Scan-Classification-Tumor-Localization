# 🧠Brain-MRI-Scan-Classification-Tumor-Localization
Early Detection of Brain Tumors using Machine Learning (SVM + PCA)

📌 Overview

This project implements a lightweight, high-accuracy Machine Learning pipeline for classifying brain MRI scans into four categories:
🧬 Glioma Tumor
🧱 Meningioma Tumor
⚪ Pituitary Tumor
🟢 No Tumor

🧭 Inspiration & Purpose

MRI-based tumor diagnosis is:
slow
prone to human error
limited by scarcity of expert radiologists
inconsistent due to MRI variations (1.5T vs 3T, noise, artifacts)

This system solves that by enabling:
⚡ Fast preliminary diagnosis
🎯 High classification accuracy
📍 Tumor region localization
🩺 Real-time second-opinion support for clinicians

🧪 Methodology & Experimental Results 
🧰Experimental Setup

Implemented using Python 3.10
Development environment: Google Colab
Key libraries used:
Scikit-Learn → ML algorithms (SVM, RF, KNN)
OpenCV → Image preprocessing & tumor localization
NumPy & Pandas → Data handling
Matplotlib & Seaborn → Visualization

Output interface: Python console + visualization plots

Hardware requirement: Standard CPU (no GPU required)

🗂️ Dataset Description
Dataset used: Brain Tumor Classification (MRI) from Kaggle

Total MRI images: 7,023
Classification labels:

🧬 Glioma

🧱 Meningioma

⚪ Pituitary Tumor

🟢 No Tumor

Image format: JPG/PNG

Dataset diversity includes:
Different magnetic field strengths (1.5T, 3T)
Noise variations
Motion artifacts

Data split strategy:
80% Training
20% Testing
Stratified Sampling to maintain class balance

📊 Performance Evaluation

Model comparison performed between:
K-Nearest Neighbors (KNN)
Random Forest (RF)
Support Vector Machine (SVM – RBF Kernel)
PCA used to reduce dimensionality while retaining 95% variance
Best performing model: SVM (RBF Kernel)

Final results:
Accuracy: 91.11%
High precision for "No Tumor" class
Minor misclassifications between Glioma & Meningioma (medically expected due to texture similarity)

Evaluation metrics included:
Accuracy
Precision
Recall
F1-score
Confusion Matrix

🚀 Future Scope

🔍 Integrate Explainable AI (Grad-CAM / LIME)
🧪 Add multi-modal MRI channels (T1, T2, FLAIR)
💻 Deploy lightweight version for hospitals without GPU
🏥 Clinical testing with real hospital data
⚡ Automatic segmentation with hybrid ML/DL models
