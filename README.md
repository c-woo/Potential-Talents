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
I will be getting word vectors for each candidates job title and comparing its cosine similarity with the word vectors from the query. The job title with the highest cosine similarity should give the closest fit to the query. I'll be checking different word embeddings to see which one performs the best. The word embeddings I'll be using are: 

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

## Conclusion
The learning to rank model after ranking with ideal candidates had a NDCG score of 0.975 for the first query and a NDCG score of 0.991 for the second query. The model is able to learn to rank more accurately when the ideal candidates have job titles that are similar to the query to begin with based on the higher NDCG score of the second query. With such a high NDCG score, I am confident in the model to correctly rerank potential candidates based on ideal candidates.


LN4UtqgLft83oTUa