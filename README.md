# 🧠 Gradient Descent in Neural Networks

> A hands-on deep learning practice project exploring gradient descent variants and the vanishing gradient problem in Artificial Neural Networks (ANNs).

---

## 📌 Overview

This project is a practical exploration of one of the most fundamental optimization concepts in deep learning — **Gradient Descent**. Through Jupyter Notebooks, this project covers the behavior of different gradient descent strategies and dives into the notorious **vanishing gradient problem**, a key challenge when training deep neural networks.

---

## 📂 Project Structure

```
Gradient-descent-in-Neural-Networks-DL-/
│
├── Batch-vs-stochastic-GD DL.ipynb   # Comparison of Batch GD vs Stochastic GD
├── vanishing-gradient DL .ipynb      # Exploration of the Vanishing Gradient problem
├── Social_Network_Ads.csv            # Dataset used for training and evaluation
└── README.md
```

---

## 📓 Notebooks

### 1. `Batch-vs-stochastic-GD DL.ipynb`
Compares two core variants of gradient descent:

| Feature | Batch Gradient Descent | Stochastic Gradient Descent |
|---|---|---|
| Update frequency | Once per epoch (full dataset) | Once per sample |
| Convergence | Stable, slower | Noisy, faster |
| Memory usage | High | Low |

Key concepts covered:
- Loss curve comparison across epochs
- Trade-offs between convergence speed and stability
- Practical implementation using the Social Network Ads dataset

---

### 2. `vanishing-gradient DL .ipynb`
Investigates the **vanishing gradient problem** — a phenomenon where gradients become extremely small during backpropagation, effectively preventing earlier layers from learning.

Key concepts covered:
- How sigmoid/tanh activations contribute to vanishing gradients
- Gradient flow visualization across network layers
- Solutions: ReLU activation, weight initialization strategies, Batch Normalization

---

## 📊 Dataset

**Social Network Ads** (`Social_Network_Ads.csv`)

A classic binary classification dataset used to predict whether a user will purchase a product based on their age and estimated salary.

| Feature | Description |
|---|---|
| `Age` | Age of the user |
| `EstimatedSalary` | Estimated annual salary |
| `Purchased` | Target label (0 = No, 1 = Yes) |

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?style=flat&logo=keras)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-yellowgreen?style=flat&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=flat)

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow keras jupyter
```

### Run Locally

```bash
# Clone the repository
git clone https://github.com/sanzidd/Gradient-descent-in-Neural-Networks-DL-.git

# Navigate into the project directory
cd Gradient-descent-in-Neural-Networks-DL-

# Launch Jupyter Notebook
jupyter notebook
```

Then open any `.ipynb` file from the Jupyter interface in your browser.

---

## 🎯 Learning Objectives

- [x] Understand how gradient descent optimizes neural network weights
- [x] Compare Batch GD vs Stochastic GD in terms of convergence and performance
- [x] Visualize and diagnose the vanishing gradient problem
- [x] Apply solutions to mitigate vanishing gradients in deep networks

---

## 📖 Key Concepts

**Gradient Descent** — An iterative optimization algorithm that minimizes a loss function by updating model parameters in the direction of the negative gradient.

**Batch GD** — Computes the gradient over the entire training dataset before updating weights. Stable but computationally expensive for large datasets.

**Stochastic GD (SGD)** — Updates weights after each individual training example. Faster and more memory-efficient, but prone to noisy updates.

**Vanishing Gradient** — As gradients are backpropagated through many layers, they can shrink exponentially, making it difficult for early layers to learn.

---

## 🙋‍♂️ Author

**Sanzid**
- GitHub: [@sanzidd](https://github.com/sanzidd)

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

> 💡 *This is a practice/learning project built to strengthen understanding of deep learning fundamentals.*
