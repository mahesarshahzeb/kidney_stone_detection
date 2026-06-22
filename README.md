# 🩺 Kidney Stone Classification

[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://https://www.kaggle.com/code/shahzaibm/kidney-stone-detection)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)

## 📌 Project Overview
This project focuses on the automated detection of kidney stones from medical imaging using Deep Learning. In the medical domain, minimizing false negatives is critical. Missing a diagnosis can lead to severe health complications. 

Therefore, the primary evaluation metric optimized for this model was **Recall**, achieving an outstanding **99.8% Recall** on the test set.

## 📊 Dataset
The dataset consists of medical images categorized into two classes:
* `0: Normal` (Healthy kidneys)
* `1: Stone` (Kidneys with identified stones)

*Data distribution is visualized in the exploratory data analysis (EDA) phase to ensure class balance and appropriate handling of the image directories.*

## 🛠️ Methodology & Tech Stack
* **Image Processing:** Python, OpenCV, PIL
* **Data Augmentation:** Utilized TensorFlow/Keras `ImageDataGenerator` to artificially expand the training dataset and prevent model overfitting.
* **Visualization:** Matplotlib and Seaborn were used for analyzing class distributions and plotting model training history.
* **Modeling:** Convolutional Neural Networks (CNNs) via TensorFlow & Keras.

## 🚀 Key Features & Pipeline
1. **Exploratory Data Analysis (EDA):** Visualizing the class distribution using Seaborn to understand the ratio of `Normal` vs. `Stone` images.
2. **Data Pipeline:** * Numerical labels are mapped to descriptive string formats (`{0: 'Normal', 1: 'Stone'}`).
   * Dynamic loading of images from directory structures using `ImageDataGenerator.flow_from_directory()`.
3. **Model Training:** Training a Deep Learning model focusing on maximizing the Recall metric.
4. **Evaluation:** Analyzing the Confusion Matrix and Classification Report to validate the 99.8% recall rate.

## 📈 Results
The model demonstrates exceptional performance in identifying positive cases of kidney stones. 

* **Recall:** **99.8%** 🏆
* High recall ensures that almost no patient with a kidney stone is misclassified as "Normal", making this model highly reliable for clinical assistance.

## 💻 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/mahesarshahzeb/kidney_stone_detection.git](https://github.com/mahesarshahzeb/kidney_stone_detection.git)
   cd kidney_stone_detection
