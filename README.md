# LLM---Detect-AI-Generated-Text
This project is part of kaggle "LLM-detect-ai-generated-text" competition . 
In this project we have build a naive bayes classifer to classify if the essay is human written or ai generated .

# Following are approach for the project 
Build a vocabulary as list:
  omit rare words for example if the occurrence is less than five times
A reverse index as the key value might be handy
  {“the”: 0, “I”:1, “happy”:2 , … }
Calculate the following probability
- Probability of the occurrence
  - P[“the”] = num of documents containing ‘the’ / num of all documents
- Conditional probability based on the class (human or LLM)
  - P[“the” | LLM]  = # of positive documents containing “the” / num of all LLM documents

Calculate accuracy using dev dataset  
 We have also experimented with different smoothing value for the model to find if there is any change in the accuracy 

- As part of analysis we tried to find top 10 words which are LLm generated and human generated .

# Enhancement for the Naive Bayes model

- As a part of enhancement we experimented few approach to improve the model accuracy for training dataset.
- We tried to impliment the NLTK  "stopwords" and "PorterStemmer" approach to check if there is any changes in the accuracy for the model.
- Also we tried to implement the TDF-IDF Vectorizer to improve the accuracy of the model .


Credits :
Chinmay Patil
Student at University of Texas At Arlington 
Computer Science
