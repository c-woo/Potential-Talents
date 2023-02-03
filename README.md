# Potential Talents

I will be attempting to rank potential job candidates based on a query and return a list of candidates that best fit the query. Once ranked I will be re-ranking candidates based on ideal candidates from the first list. 
I use a RankNet neural network model that is able to learn to rank the candidates and update it's ranking based on ideal candidates.

## Data
**Id:** Unique identifier for candidate  
**Job_title:** Job title for candidate  
**Location:** Geographical location for candidate   
**Connections:** Number of connections candidate has  
**Fit:** How fit the candidate is for the role (numeric between 0-1)

## Word Embeddings Used
* TF-IDF
* Word2Vec
* BERT
* GloVe

## Example of Model
Query Used: 'seeking human resources'

#### Fit score for word embeddings
<img src="https://i.imgur.com/oXHwya8.jpg">

#### Ranknet model
<img src="https://i.imgur.com/9Sqyf98.jpg">





LN4UtqgLft83oTUa