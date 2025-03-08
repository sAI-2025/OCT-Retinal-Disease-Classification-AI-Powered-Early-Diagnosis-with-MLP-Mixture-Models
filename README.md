# OCT-Retinal-Disease-Classification-AI-Powered-Early-Diagnosis-with-MLP-Mixture-Modelsn

## 📌 Overview
Retinal Optical Coherence Tomography (OCT) is a non-invasive imaging technique used to capture high-resolution cross-sections of the retina. With over **30 million OCT scans performed annually**, efficient analysis is critical for timely diagnosis. This project leverages an **MLP mixture model** to classify retinal diseases from OCT images with **93% accuracy**, addressing class imbalance using weighted loss functions to improve generalization.

## 🏆 Key Features
- **Automated Retinal Disease Classification** using a deep learning model.
- **Four Disease Classes**: CNV, DME, DRUSEN, and NORMAL.
- **MLP Mixture Model** optimized with **hyperparameter tuning and regularization**.
- **Handles Class Imbalance** with weighted loss functions.
- **Dataset Preprocessing and Augmentation** for improved model performance.
- **Reproducible Implementation** using Jupyter Notebooks.

---

## 📂 Project Structure
```
.
├── MLP_mixture_model.ipynb             # Main MLP mixture model implementation
├── MLP_mixture_model_in_Regulization.ipynb  # Model tuning & regularization
├── Dataset/                             # Retinal OCT dataset
│   ├── CNV/                             # Choroidal Neovascularization images
│   ├── DME/                             # Diabetic Macular Edema images
│   ├── DRUSEN/                          # Drusen images
│   ├── NORMAL/                          # Normal retinal scans
├── requirements.txt                     # Required Python dependencies
└── README.md                            # Project documentation
```

---

## 📊 About the Dataset
**Source:** Multiple hospitals and research institutions, including **Shiley Eye Institute of the University of California San Diego** and **Shanghai First People’s Hospital**.

**Dataset Composition:**
- **84,495 OCT images** categorized into **CNV, DME, DRUSEN, and NORMAL**.
- Organized into **train, validation, and test** sets.
- Each image was **expertly labeled** and verified through a multi-tier grading process involving ophthalmologists and retinal specialists.

**Data Preprocessing:**
- Images undergo **quality control** and **artifacts removal**.
- **Data augmentation** applied to enhance generalization.

---

## 🛠 Implementation Steps
### 🔹 Setup Python Environment
Ensure you have **Python 3.10** installed. Check by running:
```bash
python3 --version
```
If not installed, update Python before proceeding.

### 🔹 Install Dependencies
Use pip to install all required libraries:
```bash
pip install -r requirements.txt
```

### 🔹 Setting Up the Dataset
- Ensure the dataset is structured as shown in the **Project Structure**.
- If missing, the dataset will be **automatically downloaded** when running the notebooks.

### 🔹 Running the Model
1. Open **Jupyter Notebook** and launch `MLP_mixture_model.ipynb`.
2. Execute the notebook cells to train and evaluate the model.
3. To fine-tune hyperparameters, use `MLP_mixture_model_in_Regulization.ipynb`.

---

## 🏗 MLP Mixture Model Architecture
THere's a rewritten version of the text in a format suitable for a Git README file:
MLP-Mixer Architecture for OCT Image Classification
Overview
This repository implements an MLP-Mixer architecture designed for efficient feature extraction and classification of OCT images. The model combines the benefits of multi-layer perceptrons (MLPs) with a mixture of experts approach to handle variations in retinal OCT images.
Architecture
The MLP-Mixer architecture is based entirely on MLPs, eliminating the need for convolutions or self-attention. The model relies on basic matrix multiplication routines, data layout changes, and scalar nonlinearities.
Input: Sequence of linearly projected image patches (tokens) shaped as a "patches × channels" table
MLP Layers: Two types of MLP layers are used:
Channel-mixing MLPs: Allow communication between different channels, operating on each token independently
Token-mixing MLPs: Allow communication between different spatial locations (tokens), operating on each channel independently
Interleaving: Channel-mixing and token-mixing layers are interleaved to enable interaction between input dimensions
Key Features
Multiple Fully Connected Layers: With non-linear activations for efficient feature extraction
Dropout and Batch Normalization: To prevent overfitting and improve generalization
Weighted Loss Functions: To handle class imbalance in OCT image classification
Optimization: With Adam optimizer and learning rate scheduling for efficient training
Benefits
Improved Generalization: Through careful tuning of hyperparameters
Lower Computational Cost: Compared to complex CNN architectures
Efficient Feature Extraction: Through the use of MLPs and mixture of experts approach
---

## 📬 Contact
💡 If you have any questions or would like to collaborate, feel free to reach out:
- **Name:** Sai Krishna Chowdary Chundru
- **Email:** cchsaikrishnachowdary@gmail.com
- **GitHub:** [sAI-2025](https://github.com/sAI-2025)
- **LinkedIn:** [Sai Krishna Chowdary Chundru](https://linkedin.com/in/sai-krishna-chowdary-chundru)

🚀 If you find this project useful, give it a ⭐ on GitHub!

