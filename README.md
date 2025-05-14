# 📱 Mobile Classification Using Deep Learning

## 📌 Overview
This project leverages Convolutional Neural Networks (CNNs) to classify images of mobile phones into different brand categories. Built using TensorFlow and Keras, the pipeline handles end-to-end processing — including image preprocessing, model training, evaluation, and visualization. The dataset contains labeled mobile phone images (e.g., Apple, Samsung, Xiaomi), and the goal is to accurately identify the brand from an input image. This solution demonstrates the application of deep learning for visual classification tasks and lays the groundwork for potential deployment or integration into a mobile recommendation system.

---

## 🚀 Key Features

- 🧠 Built a custom CNN using TensorFlow and Keras for multi-class image classification.
- 🔄 Performed extensive image preprocessing (resizing, normalization, augmentation).
- 📊 Visualized training accuracy/loss and confusion matrix for performance evaluation.
- 🖼️ Displayed sample predictions with true vs. predicted labels.
- 💾 Saved the trained model for future inference or deployment.
- 📈 Achieved high accuracy on a balanced image dataset of mobile phone brands.

---

## 📂 Project Structure & Implementation

### 1️⃣ Dataset & Preprocessing
- **Dataset Format**: Images organized in folders by brand (e.g., `/dataset/apple`, `/dataset/samsung`).
- **Preprocessing**: Resized all images to uniform dimensions, normalized pixel values, and applied data augmentation (e.g., rotation, flipping) to enhance generalization.

### 2️⃣ Model Architecture
- Developed a sequential CNN model with:
  - Multiple Conv2D + MaxPooling layers
  - Flatten + Dense layers with Dropout for regularization
  - Final Softmax layer for multi-class prediction

### 3️⃣ Training & Evaluation
- Used categorical cross-entropy loss and Adam optimizer.
- Trained the model on the training set and validated on a holdout set.
- Plotted training and validation accuracy/loss to monitor overfitting.
- Generated a confusion matrix and classification report for detailed evaluation.

### 4️⃣ Prediction & Output
- Ran the model on test images to validate real-world performance.
- Visualized predictions with actual and predicted labels using Matplotlib.

---

## 📈 Key Insights

- ✅ The CNN achieved strong classification performance, demonstrating the model’s ability to learn brand-specific visual patterns.
- 🕵️ Data augmentation significantly improved generalization and helped reduce overfitting.
- 💡 Misclassifications were mostly between visually similar brands, highlighting the importance of high-quality training data.
- 🚀 The trained model is lightweight and suitable for integration into a mobile/web app for real-time image-based classification.
