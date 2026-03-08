# Sentiment Analysis on Mobile Legends Reviews (DistilBERT)

This project aims to analyze user feedback for Mobile Legends from Google Play Store reviews using Natural Language Processing (NLP) techniques. I classified reviews as Positive or Negative to understand player satisfaction and pain points.

🚀 Workflow
1. Data Cleaning
   
To ensure high-quality input for the model, the following preprocessing steps were applied:

Removal of noise (HTML tags, emojis, punctuation).

Stopwords removal and case folding.

Basic spelling correction to improve tokenization.

2. Exploratory Data Analysis (Word Analysis)

I performed frequency analysis to identify key terms in both positive and negative classes. This helped in visualizing the most common complaints and praises within the gaming community.

4. Modeling with DistilBERT

I used the DistilBERT (a distilled, faster, and lighter version of BERT) model for sentiment classification.

Input: Preprocessed user reviews.

Output: Sentiment (Positive/Negative) and Score (Confidence level between 0.0–1.0).

4. Results & Classification

The model processed the dataset with the following distribution:

Positive Reviews: 27,624

Negative Reviews: 25,027

5. Model Evaluation
   
To validate the model, I compared the Predicted Sentiments against the Real Sentiments (Ground Truth).

Ground Truth Logic: Reviews with 1-2 stars were labeled as Negative, while 4-5 stars were labeled as Positive.

Overall Accuracy: 83.8%

Detailed metrics such as Confusion Matrix, Precision, Recall, and F1-Score are included in the notebook to demonstrate the model's reliability.

🛠️ Tech Stack
Python (Pandas, NumPy)

Hugging Face Transformers (DistilBERT)

Scikit-learn (Evaluation Metrics)

Matplotlib/Seaborn (Visualizations)







