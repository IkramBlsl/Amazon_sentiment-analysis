# About Dataset

The Amazon reviews dataset consists of reviews from amazon. The data span a period of 18 years, including ~35 million reviews up to March 2013. Reviews include product and user information, ratings, and a plaintext review.

The link to the dataset : [https://www.kaggle.com/datasets/bhavikardeshna/amazon-customerreviews-polarity]

the ratings are either 1 (positive) or 2 (negative).


# 
### Training and Validation Accuracy

**Training Accuracy:**
- It is the proportion of correct predictions made by the model on the training dataset.
- It indicates how well the model has learned from the examples it was trained on.

**Validation Accuracy:**
- It is the proportion of correct predictions made by the model on the validation dataset.
- It shows how well the model can generalize to new, unseen data.

### Difference Between Training and Validation Accuracy

- **If training accuracy is much higher than validation accuracy:**
  - This may indicate overfitting, where the model memorizes the training data but does not generalize well to new data.

- **If validation accuracy is close to or higher than training accuracy:**
  - This suggests that the model generalizes well and is not overfitting.

### Batch and Epoch Concepts

**Batch:**
- A batch is a subset of the entire dataset used to train the model in one iteration.
- It allows for more frequent updates of the model weights, which can speed up training and help the model converge more quickly.
- Example: If you have 72,000 samples and use a batch size of 128, each training iteration will use 128 samples.

**Epoch:**
- An epoch is a complete pass through the entire dataset.
- If you have 72,000 samples and use a batch size of 128, there will be 72,000 / 128 = 562.5 (rounded to 563) batches per epoch.

### Number of Batches per Epoch

- The number of batches per epoch is given by the total number of samples divided by the batch size.
- Example:
  - If you have 72,000 samples and a batch size of 128:
    - Number of batches per epoch = 72,000 / 128 = 562.5 ≈ 563

### Calculation Example:

- **Dataset:** 72,000 samples
- **Batch Size:** 128
- **Number of Batches per Epoch:** 72,000 / 128 = 563 (approximately)
