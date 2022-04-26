# Text-Mining
Spam and Ham Prediciton

**Data Understanding**

https://www.kaggle.com/venky73/spam-mails-dataset


**Analytics Approach**

Make a model to predict whether an email is spam email or not.
Define appropriate metrics.
Look for the best model.

## Preprocessing

There are 6 initial stages to change the text so that each text has the same format, which is easy to process by the model :
1. we use lower() function to make all words lowercase
2. main contraction to make words that are shortened or combined into separate based on the contraction dict
3. remove number to make words without any number because text mining cannot read a number
4. remove punc to throw away a special character
5. to strip to throw away a double space
6. remove stopwords (english) to throw away a useless words
7. change every verb 2 or verb 3 words into a verb 1 or base word

## Modeling

* Tfid : 98.1%
* Vect : 97.6%
* Tfid Ngrams : 97.8%
* Vect Ngrams : 97.4%

the validation results show the logreg model that has the largest average and is quite stable, and the metrics chosen are Tfid Vectorizer without ngrams because it produces a higher score

