🧠 Alzheimer’s Disease Detection using SECNN-RF
This repository contains the implementation of a hybrid deep learning framework that leverages a Squeeze-and-Excitation Convolutional Neural Network (SECNN) combined with a Random Forest classifier to enable early and explainable diagnosis of Alzheimer’s Disease (AD) from MRI scans.

📌 Overview
Alzheimer’s Disease is a progressive neurodegenerative disorder and a leading cause of dementia. Early detection plays a critical role in improving treatment outcomes. Traditional models often fail in clinical settings due to their "black-box" nature and lack of interpretability.

This project addresses these challenges through:

Advanced feature extraction with Squeeze-and-Excitation (SE) blocks

Robust classification using Random Forest

Visual interpretability with saliency maps

Lightweight design suitable for resource-constrained environments

✅ Key Features
🧠 Early Detection: Detects AD stages (Non-Demented, Very Mild, Mild, Moderate) from MRI images.

🧬 Hybrid Model: Combines SECNN for feature extraction and Random Forest for classification.

📊 Explainable AI: Generates saliency maps to visualize important brain regions.

⚡ Efficient: Achieves high accuracy (83.06%) with fewer trainable parameters.

🧪 Robust Preprocessing: Uses data augmentation and SMOTE for class balance.

🖼️ System Architecture
Preprocessing: Image resizing (128x128x3), normalization, augmentation, SMOTE.

Feature Extraction: CNN + SE blocks with Dropout, GAP.

Classification: Feature vectors passed to Random Forest.

Explainability: Saliency maps generated for transparent decision-making.

(Replace with actual image path if available)

📂 Dataset
We use MRI brain scan images for Alzheimer’s detection. The data is preprocessed and categorized into:

Non-Demented

Very Mild Demented

Mild Demented

Moderate Demented

📁 Structure:

swift
Copy
Edit
/dataset/
  /train/
    /MildDemented/
    /ModerateDemented/
    /NonDemented/
    /VeryMildDemented/
  /test/
📈 Performance
Class	Precision	Recall	F1-Score
Mild Demented	0.82	0.87	0.85
Moderate Demented	0.97	1.00	0.98
Non Demented	0.81	0.68	0.74
Very Mild Demented	0.65	0.70	0.67

🔍 Accuracy: 83.06%

📊 Evaluation Metrics: Precision, Recall, F1-Score, Confusion Matrix

🚀 How to Run
Clone the Repository

git clone https://github.com/Krishna8660/Alzheimer-s-disease-prediction-using-Machine-Learning.git

Install Dependencies
pip install -r requirements.txt

Prepare Dataset

Organize dataset into appropriate folders as mentioned above.

Run preprocessing.py to normalize and augment data.

Train the Model

🛠️ Technologies Used
Python

TensorFlow / Keras

Scikit-learn

NumPy, Pandas

Matplotlib, Seaborn

