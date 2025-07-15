AI-Powered Molecular Toxicity Prediction (Tox21)
This project applies deep learning for molecular toxicity prediction on the Tox21 dataset. It features an automated pipeline for molecular featurization, neural network modeling, imbalance handling, robust validation, and performance visualization—all fully reproducible in Google Colab.

This README provides setup instructions, usage guidelines, and highlights the key features.

Table of Contents
Project Overview

Features

Technologies Used

Setup Instructions

Usage

Results

Troubleshooting

Future Improvements

Contributing

Output Screenshot

Project Overview
AI-Powered Molecular Toxicity Prediction leverages the Tox21 dataset to predict molecular toxicity endpoints using deep neural networks. The workflow encompasses SDF parsing, molecular fingerprinting, model training, class imbalance mitigation, and comprehensive evaluation—making it a robust, reusable tool for cheminformatics and drug discovery.

Features
Automated Molecular Featurization: Converts input molecules to ECFP (Morgan) fingerprints using RDKit.

Deep Learning Modeling: Implements dense neural network layers with dropout and class weighting for imbalanced data.

Class Imbalance Handling: Uses class weighting during training to improve minority class recall.

Robust Validation: Employs stratified K-Fold cross-validation and detailed metrics (accuracy, recall, F1, ROC-AUC).

Visualization: Generates confusion matrix, ROC curve, and other plots for model interpretability.

Google Colab Notebook: Fully annotated for transparency, reproducibility, and ease of learning.

Technologies Used
Python 3.8+

Google Colab

RDKit: Molecular parsing and fingerprinting

TensorFlow & Keras: Deep learning

NumPy & Pandas: Data manipulation

scikit-learn: Model evaluation, cross-validation

matplotlib & seaborn: Visualization

Setup Instructions
Prerequisites:

Google Account

Internet access

Steps:

Open the Colab Notebook:
https://colab.research.google.com/drive/1E6intPCIFqSfmUE-YMdb4SBf8MjED5KQ?usp=sharing

Upload Data:
Upload your SDF file to Colab or mount Google Drive as outlined in the notebook.

Install Dependencies:
Run the first code cell to install all necessary libraries (requirements.txt provided).

Usage
Run the Notebook:
Execute cells sequentially to:

Load and preprocess molecular data

Extract ECFP fingerprints

Train and validate the deep neural network

Visualize results

Interpret the Results:
Review metrics and visualizations printed in the notebook for insights.

Results
Accuracy: ~0.96

Minority Class Recall: ~0.55

Macro F1-Score: ~0.75

ROC-AUC: ~0.78
(Results will vary slightly depending on the assay endpoint and random seed)

Troubleshooting
Common Issues:

Missing or Invalid SDF: Ensure the SDF file is correctly uploaded or mounted.

RDKit Installation: Rerun the installation cell if import errors arise.

Class Imbalance: Adjust class weights or try alternative endpoints if recall is unsatisfactory.

Future Improvements
Integrate Graph Neural Networks for structure-based modeling.

Add SHAP/LIME for model explainability.

Deploy with a Streamlit or Dash dashboard for interactive use.

Incorporate multi-task learning for simultaneous prediction of multiple endpoints.

Support for other public datasets (e.g., ChEMBL).

Contributing
Contributions are welcome! Please:

Fork the repo.

Create a branch:

git checkout -b feature/your-feature

Commit your changes:

git commit -m "Add feature"

Push and open a pull request.

Output Screenshot
<img width="679" height="558" alt="image" src="https://github.com/user-attachments/assets/5e0368f4-152f-4d93-8ae6-80105992ddde" />

<img width="719" height="563" alt="image" src="https://github.com/user-attachments/assets/cb59adc4-6c68-4ed2-a85f-440e31c8facf" />


Description for Repository:
A deep learning project for molecular toxicity prediction leveraging ECFP fingerprints and neural networks on the Tox21 dataset. Handles class imbalance, robust validation, and interpretability—ready for AI-assisted drug discovery workflows.
