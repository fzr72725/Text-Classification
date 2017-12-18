# Text-Classification
Depending on which party the president is from, the topic, tone, style, vocabulary, etc. can be very different. This project is exploring over 700 presidential speeches and to find a way to identify which party (Democrat or Republican) the president is from.

## Data Set
### General Description
797 speech scripts from
45% Republican
55% Democrat
vocabulary: over 29000 unique words

### Data Dictionary

|Variable  |  Definition  |  Key|
| --- | --- | --- |
|Id  |  document id  |  |
|Path  |  document store directory  |  |
|president |  President name    |   |
|party |  Democrat or Republican   |   |

## Process
### Pre-Processing
- Tested NLTK's stemmer and lemmatizer to perform stemming/Lemmatizing on each document
- Build pipeline for vectorization and prediction

### Model Development
- LogisticRegression
- Naive Bayse
- Perform GridSearchCV to find the best hyper parameters (max_features, ngrams, etc.)
- Used PCA and NMF to discovery latent topics among documents

### Conclusion
This this particular case, Logistic Regression out-performed Naive Bayse
