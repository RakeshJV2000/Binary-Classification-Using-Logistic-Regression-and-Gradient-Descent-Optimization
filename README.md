# Binary Classification of Handwritten Digits Using Logistic Regression and Gradient Descent Optimization

The goal of this project is to implement a binary logistic regression model to classify handwritten digits from a partial dataset of the MNIST collection. The task involves distinguishing between two classes (digits '1' and '2') from 16×16 grayscale images. Each image is represented as a 256-dimensional feature vector with pixel values ranging between [-1, 1].

- Developed and trained a binary logistic regression model for classifying handwritten digits(1 and 2) from the MNIST dataset using both Gradient Descent (GD) and Stochastic Gradient Descent (SGD).
- Implemented feature extraction methods for intensity and symmetry to improve model accuracy and visualization of decision boundaries.
- Optimized hyperparameters such as learning rate and iteration number by evaluating model performance on a validation set.
- Visualized the classification results with a 2D scatter plot and decision boundary to illustrate the model's performance in separating the two classes

## Decision boundary and feature distribution
![image](https://github.com/user-attachments/assets/03a0aabd-4207-45b0-8e44-8c9bb12fecfa)

## Gradient optimization

The gradient function here computes the predicted probability 𝑝 by incorporating the true
label _𝑦 into the sigmoid function, ensuring that the prediction is adjusted based on the label. Gradient is then calculated by multiplying the error (1−𝑝) by the product of _𝑦and the feature vector _𝑥, allowing the gradient to adjust the direction of weight updates depending on the correctness of the prediction. This method ensures that correct predictions lead to smaller updates, while incorrect predictions result in larger corrections. This method is predominantly used when working with -1 and 1 labels.

## Quantitative Results:
- Achieved an accuracy of 94.44% using Gradient Descent (GD) and 97.26% using Stochastic Gradient Descent (SGD) after model training.
- SGD produced larger weight updates, resulting in faster convergence and higher accuracy compared to GD.
- The best combination of hyperparameters was found to be a learning rate of 0.1 and 100 iterations, yielding the highest validation accuracy for SGD.
