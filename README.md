# Potential Talents

I will be attempting to rank potential job candidates based on a query and return a list of candidates that best fit the query. Once ranked I will be re-ranking candidates based on ideal candidates from the first list. 
I use a RankNet neural network model that is able to learn to rank the candidates and update it's ranking based on ideal candidates.

## Data Description
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

## Example of Data
Query Used: 'seeking human resources'

<img src="https://i.imgur.com/oXHwya8.jpg">





LN4UtqgLft83oTUa