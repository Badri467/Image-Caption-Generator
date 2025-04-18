# 🧠🖼️ Image Caption Generator using CNN-LSTM

This project aims to generate meaningful captions for images using a combination of **Convolutional Neural Networks (CNNs)** for image feature extraction and **Long Short-Term Memory (LSTM)** networks for sequence generation. It leverages the **Flickr8k dataset** and implements deep learning models using TensorFlow/Keras.

---

## 📌 Problem Statement

Automatically generating a descriptive caption for a given image is a complex task that requires understanding both visual elements and natural language. This project bridges **computer vision** and **natural language processing** by generating captions using a deep learning pipeline.

---

## 🎯 Objectives

- Extract rich features from images using a pre-trained CNN (InceptionV3).
- Use LSTM networks to generate captions based on these features.
- Train and evaluate the model on the Flickr8k dataset.
- Generate captions for new, unseen images.

---

## 🛠️ Methodology

### 📁 Dataset
- **Flickr8k**: Contains 8,000 images with 5 captions each.
- Only a subset is used due to computational constraints.

### ⚙️ Preprocessing
- Text:
  - Tokenization, padding, vocabulary creation.
  - Addition of `<start>` and `<end>` tokens.
- Images:
  - Resized and preprocessed to match InceptionV3 input format.
  - Features extracted using pre-trained InceptionV3.

### 🧱 Model Architecture
- **CNN (InceptionV3)**: Extracts image features.
- **Embedding Layer**: Converts input sequences into dense vectors.
- **LSTM**: Generates sequences (captions).
- **Dense Layer**: Predicts the next word using softmax.

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Image-Caption-Generator.git
   cd image-caption-generator
