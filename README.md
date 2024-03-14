# SST-Text-Classification-using-Naiive-Bayes

## Introduction
In this project, I implemented a Naive Bayes classifier from scratch to classify text samples into five distinct sentiment classes using the Stanford Sentiment Treebank (SST) dataset. I also computed the confusion matrix and evaluated the classifier's performance using precision, recall, and F1 score.

![image](https://github.com/SaadElDine/SST-Text-Classification-using-Naiive-Bayes/assets/113860522/e361a821-be24-411a-8b25-4d9f6bfa4038)


## Dataset Description
The SST dataset consists of movie reviews labeled with sentiment scores ranging from 0 to 1. We mapped these scores to five classes: very negative, negative, neutral, positive, and very positive.

## Naive Bayes Classifier Implementation
### Training
- We implemented the `train_naive_bayes` function to calculate the prior probabilities and likelihood probabilities for each class based on the training data.
- The function computes the log prior probabilities and log likelihoods of each word in the vocabulary for each class.

  ![image](https://github.com/SaadElDine/SST-Text-Classification-using-Naiive-Bayes/assets/113860522/1b82336f-c9b8-48af-bfb0-a3aaed323b09)


### Testing
- The `test_naive_bayes` function predicts the class for each test sample based on the computed probabilities.
- It calculates the log likelihood of each word in the test sample for each class and selects the class with the highest total log likelihood as the prediction.

  ![image](https://github.com/SaadElDine/SST-Text-Classification-using-Naiive-Bayes/assets/113860522/a29f0c75-5119-432d-b936-7798a989f36a)


## Confusion Matrix
- We computed the confusion matrix to evaluate the classifier's performance.
- The confusion matrix shows the counts of true positives, false positives, true negatives, and false negatives for each class.

  ![image](https://github.com/SaadElDine/SST-Text-Classification-using-Naiive-Bayes/assets/113860522/cb7fa42e-3f0f-4a91-a0bc-191a32408e2f)


## Evaluation Metrics
- We calculated precision, recall, and F1 score per class using the confusion matrix.
- Additionally, we computed the macro-averaged precision, recall, and F1 score to evaluate the overall performance of the classifier.

## Results and Comparison
- Our custom Naive Bayes implementation achieved reasonable performance on the SST dataset.
- We compared our results with scikit-learn's implementation, which showed similar performance but with slight differences in some metrics.

  ![image](https://github.com/SaadElDine/SST-Text-Classification-using-Naiive-Bayes/assets/113860522/c8282090-1bed-433c-8541-b26bce2150bb)


## Conclusion
In conclusion, our Naive Bayes classifier successfully classified text samples into sentiment classes, demonstrating the effectiveness of the algorithm for sentiment analysis tasks. Further optimizations and experiments could be conducted to improve the classifier's performance. For detailed code implementation and results, please refer to the provided Python code.
