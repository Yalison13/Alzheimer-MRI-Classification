# Alzheimer-MRI-Classification

## 📖 Project Overview
This repository implements a deep learning pipeline to classify MRI images into four stages of Alzheimer's Disease (Mild Demented, Moderate Demented, Non Demented, and Very Mild Demented). By leveraging **Transfer Learning** with a pre-trained **DenseNet201** model, this project achieves efficient and accurate diagnostic classification.



## 🚀 Key Features
* **Transfer Learning:** Utilizes DenseNet201 weights pre-trained on ImageNet to enhance feature extraction performance on medical imaging.
* **Data Preprocessing:** Implements `ImageDataGenerator` for real-time data augmentation, addressing class imbalance common in medical datasets.
* **Performance Metrics:** The model's efficacy is evaluated using accuracy scores and confusion matrices to visualize classification precision across all categories.

## 🛠️ Tech Stack
* **Framework:** TensorFlow 
* **Architecture:** DenseNet201 (Transfer Learning)
* **Preprocessing:** `ImageDataGenerator`
* **Visualization:** Matplotlib, Seaborn, Scikit-learn
* **Environment:** Google Colab

## 📊 Results
The model was evaluated on a test set to ensure robustness. Below is a representation of the classification performance.
<p align="center">
  <img src="https://github.com/Yalison13/Alzheimer-MRI-Classification/blob/main/results/Confusion%20Matrix.png?raw=true" width="75%">
  <br>
  <b>Figure 1: Confusion Matrix for Alzheimer's classification using DenseNet201.</b>
</p>

<p align="center">
	<img src="https://github.com/Yalison13/Alzheimer-MRI-Classification/blob/main/results/Accuracy.png?raw=true" width = "75%">
	<br>
	<b>	Figure 2: Training and Validation Accuracy curves.</b>
</p>

<p align="center">
	<img src="https://github.com/Yalison13/Alzheimer-MRI-Classification/blob/main/results/Loss.png?raw=true" width = "75%">
	<br>
	<b>	Figure 3: Training and Validation Loss evolution.</b>
</p>



**Model Architecture:** DenseNet201 (Frozen base layers with custom dense head)
**Optimizer:** Adam
**Loss Function:** Categorical Crossentropy


## ⚙️ Getting Started

### Running on Google Colab (Recommended)
Since this project is developed in a Jupyter Notebook format, the easiest way to run it is directly in Google Colab.

1. **Open in Colab:** Upload `notebooks/Alzheimer_Training.ipynb` to Google Colab)
2. **Kaggle Setup:** As this project uses a Kaggle dataset, ensure you upload your `kaggle.json` API key to the Colab environment when prompted, or configure it via Colab's secrets menu.
3. **Run All:** Simply click "Run all" to execute the training pipeline.

