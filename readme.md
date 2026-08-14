# Improving Customer Satisfaction: Sentiment Analysis on Customer Feedback for an App Designed for Online Classes and Video Conferencing Using BERT



## Objective
The objective of this project is to improve customer satisfaction by performing sentiment analysis on customer feedback for an app designed for online classes and video conferencing. The analysis will be conducted using BERT (Bidirectional Encoder Representations from Transformers), a state-of-the-art natural language processing model.

## Data
The initial dataset consisted of customer feedback collected from users of the app. However, all the rows were initially labeled as 1, indicating positive sentiment, and there were no rows labeled as 0, indicating negative sentiment. To address this issue, sentiment analysis was performed on the dataset, and the rows were labeled as 1 and 0 based on the sentiment expressed in the text. To improve the representation of negative sentiment, negation generation techniques were applied. 

Due to the initial class imbalance, where positive labels were more prevalent than negative labels, oversampling techniques were employed to balance the dataset. This involved creating additional instances of the positive class to match the number of instances in the negative class.

## Methodology
The project utilizes BERT, a pre-trained language model known for its contextual understanding of text. BERT was fine-tuned using the sentiment-labeled dataset to train a sentiment analysis model. Fine-tuning involves updating the model's parameters using the specific task of sentiment analysis on the customer feedback data.


## Key Features
- Performed sentiment analysis on the initial dataset, labeling rows as 1 and 0 based on the sentiment expressed in the text.
- Utilized NLP techniques including Spacy, NLTK, and TensorFlow for sentiment analysis and machine learning.
- Utilized Plotly and Word Cloud for exploratory data analysis (EDA) to gain insights into the customer feedback dataset.
- Applied negation generation techniques to enhance the representation of negative sentiment in the dataset.
- Addressed class imbalance by oversampling the positive class to achieve a balanced dataset.
- Tuned the model for high precision in identifying positive sentiments and high recall in identifying negative sentiments.
- Developed a BERT-based model for sentiment analysis on a balanced dataset, achieving an accuracy of 84% with a focus on high precision for positive sentiments and high recall for negative sentiments.


## Classification Results

The sentiment analysis model achieved the following performance metrics on the test dataset:

          precision    recall  f1-score   support

       0       0.95      0.70      0.80       659
       1       0.77      0.97      0.86       702
          
          accuracy                 0.84      1361


The precision, recall, and F1-score are commonly used metrics to evaluate the performance of a binary classification model. In this case, class 0 represents negative sentiments and class 1 represents positive sentiments.

The model achieved an accuracy of 84%, indicating the percentage of correctly classified instances out of the total test dataset. The precision for class 0 is 95%, meaning that when the model predicted a sentiment as negative, it was correct 95% of the time. The recall for class 1 is 97%, indicating that the model successfully identified 97% of the positive sentiments in the dataset. The F1-score combines precision and recall, providing a single metric to assess the model's overall performance.

These results suggest that the sentiment analysis model has a good ability to classify customer feedback accurately, with a focus on correctly identifying positive sentiments.
