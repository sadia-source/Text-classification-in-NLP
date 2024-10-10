# Project Title

Text classification in NLP (Natural Language Processing)

# Problem Statement
With the rapid rise of digital communication via emails and SMS, spam detection has become crucial for filtering out unwanted or harmful content. In this project, I will use the text data from the spam.tsv dataset to develop a model that can accurately classify messages as either "spam" or "ham."

# Overview
The spam.tsv dataset is designed for a classic spam detection task, where we aim to classify text messages as either "spam" or "ham" (not spam). This dataset contains two columns:

Class: The target label, indicating whether a message is "spam" or "ham.
Message: The text content of the message that needs to be analyzed.
The goal is to build a text classification model that can predict whether a given message is spam or ham based on its content

# Data Preprocessing Steps
# 1.Lowercasing:
All the text in the messages was converted to lowercase. This helps standardize the data by removing case sensitivity. For example, "Free" and "free" are treated as the same word.

# 2. HTML Tag Removal:
Any HTML tags (e.g.) were stripped out from the text. This is crucial when dealing with text that might have been scraped from websites or contains formatting markup.

# 3.Punctuation Removal:
I removed punctuation marks (like commas, periods, and exclamation points) from the messages. Punctuation does not usually contribute to understanding the intent of a message and can be safely removed to reduce noise.

# 4.Text Vectorization using CountVectorizer:
After cleaning the text, I converted it into numerical form using the CountVectorizer technique. This method transforms the text into a matrix where each row corresponds to a message, and each column corresponds to a word (or token). The value in each cell represents how many times the word appears in the message.#
 # Conclusion: 
 I built a spam detection model using the spam.tsv dataset. After preprocessing (lowercasing, punctuation/HTML removal, and label encoding), I used CountVectorizer for feature extraction. The Multinomial Naive Bayes model achieved 98% accuracy, effectively classifying messages as spam or ham. Additionally, I implemented a solution to predict spam/ham for future messages
