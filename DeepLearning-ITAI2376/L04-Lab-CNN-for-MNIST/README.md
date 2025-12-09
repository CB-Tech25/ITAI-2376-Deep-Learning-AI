# 💻 Lab L-04: Building and Optimizing a CNN for MNIST Classification

## Overview

[cite_start]This assignment involved implementing and optimizing a Convolutional Neural Network (CNN) using **TensorFlow/Keras** to classify handwritten digits from the **MNIST dataset**[cite: 1, 4, 5]. [cite_start]The focus was on understanding the role of each layer and the impact of hyperparameter tuning[cite: 7, 9].

**Keywords:** CNN, MNIST, Computer Vision, Keras, TensorFlow, Feature Extraction, Hyperparameter Tuning.

---

## 🚀 Architecture and Performance

### Final Model Structure

[cite_start]The core architecture mirrored a mini LeNet-5, achieving near state-of-the-art results for a basic CNN on MNIST[cite: 29, 30]:

* [cite_start]**Final Accuracy:** 99.21% on the test set[cite: 30].
* [cite_start]**Architecture:** Two Conv2D layers (32 and 64 filters), two MaxPooling2D layers, Flatten, Dropout (0.5), and a final Dense (10 classes, Softmax) layer[cite: 29].
* [cite_start]**Optimization:** **Adam** optimizer and **Categorical Cross-Entropy** loss[cite: 23, 22].

### Key Learnings from Experimentation

* [cite_start]**Model Complexity vs. Efficiency:** Increasing the number of filters from 64 to 128 boosted accuracy from 0.9921% to 0.9935%, but significantly increased training time due to the jump in parameters (from 34k to over 100k)[cite: 12, 13].
* [cite_start]**Translational Invariance:** Removing a **MaxPooling2D** layer led to overfitting, confirming its role in downsampling feature maps, reducing dimensions, and contributing to translational invariance[cite: 14, 16].
* [cite_start]**Preprocessing is Crucial:** Normalizing pixel values to `[0, 1]` was essential to stabilize training, as unnormalized data caused exploding gradients (NaN losses) in initial runs[cite: 17, 19].
* [cite_start]**Regularization:** The **Dropout** layer (rate=0.5) was confirmed to be critical, preventing overfitting and forcing the model to learn more robust features[cite: 27].

---

## 💡 Conclusion

[cite_start]This lab successfully demystified CNNs, showing they are not "black boxes" but layered systems for **hierarchical feature extraction**[cite: 32]. [cite_start]The most important takeaway was that **experimentation is key**; tweaking parameters revealed how small changes ripple through performance, emphasizing iterative design in AI[cite: 33].

---

## 📚 Repository Files

* `L04-CNN-MNIST-Code.ipynb`: The Jupyter Notebook containing the code, training logs, and reflection answers.
* `L04-Courtneybernard-reflective journal.docx`: The final written reflection document.
* `README.md`: This documentation file.
