## Bagging with Decision Trees on MNIST Dataset

This project implements a Bagging ensemble method using Decision Trees to classify images from the MNIST dataset. The code demonstrates the process of training three decision trees on different subsets of the training data, making predictions on the test set, and evaluating the model's performance using an accuracy and confusion matrix.

## Project Structure

- **main.py**: The main Python script containing the logic for loading the MNIST dataset, bagging, training decision trees, and evaluating the model.
- **README.md**: This file.

## Libraries Used

- `numpy`: For array manipulation and mathematical operations.
- `matplotlib`: For visualizing images and confusion matrices.
- `seaborn`: For plotting heatmaps of the confusion matrix.
- `sklearn`: For loading the MNIST dataset, implementing decision trees, and calculating accuracy and confusion matrix.

## Dataset

The project uses the MNIST dataset, which consists of 70,000 28x28 grayscale images of handwritten digits (0-9). It is loaded from OpenML using the `fetch_openml()` function from the `sklearn.datasets` module.

## Approach

1. **Data Preprocessing**:
   - The MNIST dataset is divided into training and test sets, with the first 60,000 samples used for training and the remaining 10,000 used for testing.

2. **Bagging**:
   - The bagging method involves creating random subsets of the training data by randomly sampling from the original dataset with replacement.
   - Three different bags are created, and a decision tree classifier is trained on each bag.

3. **Majority Voting**:
   - Each decision tree makes a prediction on the test data. A majority vote is used to determine the final prediction.

4. **Evaluation**:
   - The accuracy of the model is calculated by comparing the predicted labels with the true labels from the test set.
   - A confusion matrix is plotted to visualize the performance of the model.

Acknowledgments
The MNIST dataset is publicly available from OpenML and was used for benchmarking machine learning algorithms.
vbnet

Make sure to replace `yourusername` with your actual GitHub username, and you may need to adjust any project details (e.g., files, licenses) based on your actual project structure.





