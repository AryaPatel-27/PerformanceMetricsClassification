# Performance Metrics for Classification

## Workshop Overview

This workshop focuses on understanding classification and different performance metrics used to evaluate classification models.

The MNIST dataset is mainly used in this workshop. It contains images of handwritten digits from 0 to 9. The workshop first changes the MNIST problem into a binary classification problem where the model predicts whether an image represents the digit 5 or not.

The workshop also includes an exercise using the Fashion-MNIST dataset to apply a similar classification process.

## Objectives

The main objectives of this workshop are to:

- Understand classification and classifiers
- Understand binary classification
- Train a classification model
- Use cross-validation to evaluate a model
- Understand accuracy and its limitations
- Compare a trained classifier with a `DummyClassifier`
- Understand the confusion matrix
- Calculate and interpret precision and recall
- Understand the F1 score
- Understand the trade-off between precision and recall
- Observe how changing the classification threshold affects precision and recall
- Apply the classification process to Fashion-MNIST

## Dataset

The main dataset used in this workshop is the **MNIST dataset**.

MNIST contains 70,000 grayscale images of handwritten digits from 0 to 9. Each image is 28 × 28 pixels and is represented using 784 pixel values.

The dataset is divided into:

- 60,000 training images
- 10,000 testing images

For binary classification, the target labels are changed so that:

- `True` represents the digit 5
- `False` represents any digit other than 5

## Models Used

The workshop uses classification models from Scikit-learn, including:

- `SGDClassifier`
- `DummyClassifier`
- `RandomForestClassifier`

The `SGDClassifier` is used to train a binary classifier that determines whether a handwritten digit is 5 or not.

The `DummyClassifier` is used as a simple baseline for comparing the performance of the trained classifier.

## Performance Metrics

Different methods and performance metrics are explored in this workshop.

### Accuracy

Accuracy shows how many predictions made by the classifier are correct compared with the total number of predictions.

Cross-validation is also used to evaluate the model on different parts of the training data.

### Confusion Matrix

A confusion matrix helps us understand the predictions of a classifier in more detail. It shows:

- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

### Precision

Precision measures how many of the samples predicted as positive are actually positive.

High precision is useful when false positive predictions should be minimized.

### Recall

Recall measures how many of the actual positive samples were correctly identified by the classifier.

High recall is important when missing a positive case can have serious consequences.

### F1 Score

The F1 score combines precision and recall into a single performance measure. It is useful when both precision and recall are important.

### Precision-Recall Trade-off

The workshop also demonstrates that changing the classification threshold affects precision and recall.

Increasing or decreasing the threshold changes how easily the classifier predicts a sample as positive. Therefore, the appropriate threshold depends on the requirements of the problem.

## Fashion-MNIST Exercise

The classification process is also applied to the Fashion-MNIST dataset. This exercise provides practice with preprocessing data, training a classifier, and evaluating its performance on another image classification dataset.

## Key Insights

From this workshop, we learned that accuracy alone may not always provide enough information about the performance of a classifier.

Metrics such as precision, recall, F1 score, and the confusion matrix provide more information about the types of correct and incorrect predictions made by a model.

We also learned that the importance of precision and recall depends on the real-world problem. In some situations, reducing false positives is more important, while in other situations, identifying as many actual positive cases as possible is more important.

Overall, this workshop helped us understand how different classification performance metrics can be used to evaluate machine learning models.

## Technologies and Libraries

- Python
- Jupyter Notebook
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Installation

Install the required Python packages using:

```bash
pip install -r requirements.txt
```

## Running the Workshop

1. Clone this repository.
2. Install the required packages.
3. Open `PerformanceMetricsClassification.ipynb`.
4. Select the appropriate Python environment or kernel.
5. Run the notebook cells in order.

## Team

This workshop was completed as a group exercise for the Applied Artificial Intelligence & Machine Learning program at Conestoga College.