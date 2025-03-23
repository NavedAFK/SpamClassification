# SpamClassification
**Spam Classification Using LSTM**

**Project Overview**
This project focuses on building a Spam Classification Model using a Recurrent Neural Network (RNN) with an LSTM (Long Short-Term Memory) architecture. The objective is to accurately classify messages as either Spam or Ham (legitimate) while ensuring a well-documented approach that highlights preprocessing, model architecture, and performance evaluation.

**Dataset Description** 
Dataset: spam.csv containing SMS messages labeled as spam or ham.

Columns:
v1 - Label (ham/spam)
v2 - Text message
Unnamed: 2, Unnamed: 3, Unnamed: 4 - Dropped due to irrelevance.


**Preprocessing and Data Cleaning**
The following preprocessing steps were applied to ensure clean and standardized data:
Dropped unnecessary columns.
Converted text to lowercase and removed punctuations.
Encoded labels as binary values (ham = 0, spam = 1).
Tokenized and padded sequences to ensure uniform input size for the model.

**Model Architecture**
The spam classifier is built using an LSTM-based architecture:
Embedding Layer: Converts text to dense vector representations.
Bidirectional LSTM Layer: Captures contextual information in both forward and backward directions.
Dense Layer with ReLU Activation: For feature extraction.
Dropout Layer: Prevents overfitting.
Output Layer with Sigmoid Activation: Generates binary classification output.

**Evaluation Metrics**
To assess the model’s performance, the following metrics were used:
Accuracy: Overall correctness of predictions.
Precision: Measures the proportion of predicted spam that is truly spam.
Recall: Assesses the model's ability to detect spam.
F1-Score: Balances precision and recall for a more comprehensive performance evaluation.
Confusion matrix visualization was also used to better understand the classification results.

**How to Run the Project**
Clone the Repository: Download or clone the project repository to your local system.
Install Required Packages: Ensure that necessary dependencies (TensorFlow, Pandas, Scikit-learn, etc.) are installed.
Run the Model: Execute the Python script to train, evaluate, and test the model.
Test and Predict: Use the saved model to classify new messages as spam or ham.

**Results and Performance**
The final model demonstrated high performance with the following results:
High accuracy and balanced precision-recall scores.
Low false positive and false negative rates, ensuring reliable spam detection.
Consistent results on both training and validation datasets.

