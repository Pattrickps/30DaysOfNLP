# 30DaysOfNLP

<h2> Day 6 </h2> – 

<p><b>Shallow transfer learning for NLP</b> - 
The topic covered today is Shallow transfer learning for NLP. It’s all about using pre-trained embedding in a semi-supervised manner to transfer pre-trained knowledge to a problem.

Analyzed the performance of embeddings like Word2Vec and Sent2Vec on the IMDB review dataset.
We can get Word2Vec embedding either using CBOW or Skip-Gram model. Both of these have their own pros and cons. Also, the major weakness of Word2Vec is it's inability to handle OOV( Out of Vocab ) words. But while using Sent2Vec we need not worry about OOV words.

Also came across another very interesting pre-trained shallow Neural Net based technique called FastText which attempts to enhance Word2Vec by repeating the Skip-Gram methods on the character n-grams, which allows it to handle OOV words during inference phase. (The embeddings generated for sub-word character n-grams enables it build embedding for unseen words by simply aggregating these char n-gram embeddings).

Both FastText and the Word2Vec can be implemented using the Gensim toolkit. However , for using Sent2vec we need to make use of the Sent2vec library https://github.com/epfml/sent2vec
</p>
