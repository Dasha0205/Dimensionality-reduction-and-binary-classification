# Dimensionality reduction and binary classification

This project explores classification and data analysis on the Fashion MNIST dataset using various machine learning models and dimensionality reduction techniques. The goal is to build, compare, and optimize classifiers to achieve robust performance on grayscale images of fashion items.

## Dataset

* **train.csv**: Training data containing 28x28 grayscale images with labels.
* **evaluate.csv**: Test data without labels, used for final prediction.

## Project Tasks and Methods

1. **Data Loading and Exploration**

   * Loaded and split the training dataset into subsets for training, validation, and testing.
   * Performed exploratory data analysis (EDA) including visualization of sample images.

2. **Modeling and Evaluation**
   Applied and compared the following classifiers:

   * Support Vector Machine (**SVM**) with multiple kernel functions
   * Naive Bayes Classifier (**generative model**)
   * Linear Discriminant Analysis (**LDA**)

   For each model:

   * Discussed suitability for image classification tasks.
   * Tuned key hyperparameters to optimize performance.
   * Analyzed and commented on results.

3. **Data Generation Using Generative Models**

   * Used trained Naive Bayes or LDA models to generate synthetic data points per class.
   * Transformed generated data back to 28x28 images and evaluated their quality.

4. **Dimensionality Reduction Techniques**

   * Applied Principal Component Analysis (**PCA**) and Locally Linear Embedding (**LLE**).
   * Repeated classification steps on reduced-dimensional data to assess performance improvements.
   * Investigated optimal number of dimensions for best accuracy.

5. **Final Model Selection and Prediction**

   * Selected the best-performing model based on validation results.
   * Estimated expected accuracy on unseen data.
   * Generated predictions for the test set (`evaluate.csv`).
   * Created `results.csv` with predicted labels and corresponding IDs.
