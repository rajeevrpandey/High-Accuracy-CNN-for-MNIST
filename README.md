# **MNIST Handwritten Digit Classification using CNN**

## **Overview**
This project builds and trains a **Convolutional Neural Network (CNN)** to classify handwritten digits (0-9) using the **MNIST dataset**. The model is implemented using **TensorFlow and Keras** and achieves high accuracy by leveraging convolutional layers, pooling, and dropout for regularization.

## **Dataset**
The **MNIST dataset** consists of **60,000 training images** and **10,000 test images** of handwritten digits. Each image is **28x28 pixels** in grayscale.

## **Project Features**
✅ Loads and preprocesses the MNIST dataset  
✅ Normalizes pixel values to the range **[0,1]**  
✅ Splits data into **training (55,000), validation (5,000), and test (10,000) sets**  
✅ Implements a **CNN** with **Conv2D, MaxPooling, Dense, and Dropout layers**  
✅ Trains the model using the **Nadam optimizer** and evaluates on test data  

---

## **Model Architecture**
The CNN model consists of:
1. **Conv2D (32 filters, 3×3, ReLU, "same" padding)**  
2. **Conv2D (64 filters, 3×3, ReLU, "same" padding)**  
3. **MaxPooling2D (2×2 pooling layer)**  
4. **Flatten (converts 2D feature maps into a 1D vector)**  
5. **Dropout (25% to reduce overfitting)**  
6. **Dense (128 neurons, ReLU activation)**  
7. **Dropout (50% for regularization)**  
8. **Dense (10 neurons, Softmax activation for classification)**  

---

## **Results**
The model achieves high accuracy on the MNIST dataset:

Training Accuracy: **~99%**  
Validation Accuracy: **~98%**  
Test Accuracy: **~98%**
