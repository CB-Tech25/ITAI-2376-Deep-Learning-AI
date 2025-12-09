# 🧠 Project A-03: Neural Network Zoo Implementation

## Overview

This repository contains the full implementation of the **Neural Network Zoo** assignment for the ITAI-2376 Deep Learning course. The project focuses on building and comparing the performance of multiple fundamental neural network architectures to solve a [Classification/Regression] problem.

**Keywords:** Multi-Layer Perceptron (MLP), Convolutional Neural Network (CNN), Recurrent Neural Network (RNN), [Other architecture used].

## Problem Statement

The goal was to [Clearly state the project goal, e.g., classify handwritten digits from the MNIST dataset] using a variety of network structures to understand the trade-offs in complexity, training time, and performance (accuracy/loss).

## Methodology

This project includes the implementation of the following architectures:

* **Multi-Layer Perceptron (MLP):** Used as the baseline model with [Number] hidden layers.
* **Convolutional Neural Network (CNN):** Designed with [Number] convolutional blocks for feature extraction.
* **[Third Architecture, e.g., Simple RNN]:** Implemented to handle sequential data aspects of the dataset.

All models were trained using the [Optimizer, e.g., Adam Optimizer] with a learning rate schedule and evaluated using [Metric, e.g., F1-Score/Accuracy].

## Key Results

The following table summarizes the performance of the implemented models on the test set:

| Architecture | Accuracy/F1-Score | Loss | Key Takeaway |
| :--- | :--- | :--- | :--- |
| MLP Baseline | [X.XX]% | [Y.YY] | Fast training, limited performance on complex features. |
| CNN Model | [A.AA]% | [B.BB] | Highest feature extraction capability and overall performance. |
| RNN Model | [C.CC]% | [D.DD] | Provided insight into sequential handling, but not optimal for this task. |

Visualizations, including training history and confusion matrices for the best-performing model (CNN), are available in the **[results/](results/)** directory.

## Repository Structure & Files

| File/Folder | Description |
| :--- | :--- |
| [`neural_network_zoo_code.ipynb`](neural_network_zoo_code.ipynb) | **Core Code:** Contains all model definitions, training loops, and evaluation logic. |
| `supporting_functions.py` | Utility scripts for data loading and plotting. |
| `NN-Zoo-Report.pdf` | The final written report summarizing theoretical concepts and findings. |
| `results/` | Contains output visualizations (e.g., model summaries, loss curves). |

### Requirements & Setup

To run this code locally, you will need the following dependencies:
* Python 3.x
* PyTorch (or TensorFlow)
* NumPy
* Matplotlib

* ## Collaboration

This project was completed as a group assignment. All collaborators are credited in the official report header (`NN-Zoo-Report.pdf`).

**My Primary Contribution:** I was responsible for **designing and implementing the CNN and RNN architectures,** running hyperparameter tuning experiments, and generating the final performance metrics and visualizations.
