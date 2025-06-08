# 🕶️ Spectacles Detection using VGG16 (Transfer Learning)

This project is a binary image classification model that detects whether a person in a given image is **wearing spectacles** or **not**. It uses **Transfer Learning with VGG16**, a powerful pretrained convolutional neural network from the ImageNet dataset.

---

## 📌 Overview

- **Task**: Classify images as "With Glasses" or "Without Glasses"
- **Model**: VGG16 (pretrained on ImageNet)
- **Technique**: Transfer Learning
- **Framework**: TensorFlow / Keras
- **Notebook**: Developed and tested using Google Colab

---

## 🧠 Model Architecture

- **Base**: VGG16 (include_top=False, weights='imagenet')
- **Image Size**: 224x224 (required by VGG16)
- **Custom Top Layers**:
  - `GlobalAveragePooling2D`
  - `Dense(128, activation='relu')`
  - `Dropout`
  - `Dense(1, activation='sigmoid')` (for binary output)
- **Loss**: Binary Crossentropy
- **Optimizer**: Adam
- **Metric**: Accuracy

---

## 🧪 Dataset

- **Source**: [Kaggle - People with and without Glasses](https://www.kaggle.com/datasets/ashwingupta3012/people-with-and-without-glasses)
- **Categories**: 
  - `WithGlasses/`
  - `WithoutGlasses/`
- Images were preprocessed (resized, normalized) and loaded using `ImageDataGenerator`.

---

## 📈 Training Results

- Achieved over **X% training accuracy** and **Y% validation accuracy**
- Successfully tested on real-world images

---

## 🧪 How to Use

1. Open the `spectacles_classifier_vgg16.ipynb` notebook in Google Colab.
2. Upload the dataset (or mount from Google Drive).
3. Run the cells to train and evaluate the model.
4. Use the `predict_glasses()` function to test new images.

---

## 📁 Files in This Repository


---

## 🙌 Acknowledgements

- [Kaggle Dataset](https://www.kaggle.com/datasets/ashwingupta3012/people-with-and-without-glasses)
- [VGG16 Documentation (Keras)](https://keras.io/api/applications/vgg/)

---

## 👨‍💻 Author

**Arup Amlan**  
B.Tech Student | ML & Deep Learning Enthusiast  
---
