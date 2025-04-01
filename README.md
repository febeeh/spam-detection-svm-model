# spam-detection-svm-model
This repository features a highly accurate spam detection model trained using a Support Vector Machine (SVM). It includes a pre-trained model file and an IPython Notebook for execution.

## Model Perfomance
* This SVM model achieves high accuracy in detecting spam emails.
* It is trained on a well-processed dataset to optimize performance.
* The model effectively reduces false positives and enhances precision in spam classification.

## Model Usage: Spam Email Detection
This model is designed to classify emails as spam or not spam using an SVM classifier.

### Steps to Use the Model:
#### 1: Load the trained model and vectorizer
```python
import joblib
tfidf = joblib.load('tfidf_vectorizer.pkl')
classifier = joblib.load('spam.model')
```
#### 2: Prepare your input text
```python
input_text = ["Congratulations! You won a prize."]
input_tfidf = tfidf.transform(input_text)
```
#### 3: Make a prediction
```python
prediction = classifier.predict(input_tfidf)
print(prediction)
```

### Executing the Jupyter Notebook
The provided Jupyter Notebook ```(spam_detection.ipynb)``` contains step-by-step instructions to test the model. Follow these steps to execute it:
#### 1: Open the notebook:
```jupyter notebook spam_detection.ipynb```
#### 2: Run all cell

______________________________________________

## Done
