# Perceptron Model Implementation and Loss Function Exploration

## Overview

This project implements a **Perceptron model** for binary classification. Additionally, the project explores various loss functions using **SGDClassifier**, which optimizes weights more efficiently with stochastic gradient descent (SGD). The dataset used for this project is located in the `data` folder.

### Key Tasks:

- Implementation of the Perceptron model.
- Exploration of other loss functions using `SGDClassifier`, such as **Perceptron loss** and **Binary Cross Entropy (log loss)**.
- Hyperparameter tuning using `GridSearchCV` to optimize the baseline Perceptron model.

The results show that the **Perceptron loss** performed better than **Binary Cross Entropy** in terms of classification accuracy.

## Project Structure

- **`data/diabetes.csv`**: The dataset used for training and testing the models.
- **`perceptron.ipynb`**: The Jupyter notebook that contains the full implementation of the Perceptron model, loss function exploration, and hyperparameter tuning.

## Approach

### Perceptron Model:

- A simple **Perceptron model** was implemented as a baseline for binary classification.
- The model was trained by minimizing misclassifications using **Perceptron loss**.

### Loss Function Exploration:

- **SGDClassifier** was employed to experiment with additional loss functions:

  - **Perceptron loss**: The loss used by the baseline model.
  - **Binary Cross Entropy (Log Loss)**: Used for logistic regression.

  `SGDClassifier` with stochastic gradient descent helps speed up the training process by updating weights with each sample instead of the whole dataset at once.

### Hyperparameter Tuning:

- **GridSearchCV** was used to tune hyperparameters of the Perceptron model:
  - Learning rate (`eta0`)
  - Regularization strength (`alpha`)
  - Penalty terms (`l1`, `l2`, `elasticnet`)
- The tuning helped improve the model performance. The results showed that **Perceptron loss** performed better than **Binary Cross Entropy loss** for this dataset.

## Results

- **Perceptron Loss**: Achieved higher accuracy and better classification performance.
- **Binary Cross Entropy Loss**: While common in logistic regression, it was outperformed by the Perceptron loss for this specific task.

## How to Run

1. **Clone this repository**:

   ```bash
   git clone https://github.com/tusharbansal842/Diabetes-Prediction-Using-Perceptron.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd Diabetes-Prediction-Using-Perceptron
   ```

3. **Open the Jupyter notebook to view and run the code**:

   ```bash
   jupyter notebook perceptron.ipynb
   ```
