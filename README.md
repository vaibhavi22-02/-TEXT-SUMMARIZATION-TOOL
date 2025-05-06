# TEXT-SUMMARIZATION-TOOL

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: VAIBHAVI SHINGARE

*INTERN ID*: CT06DA723

*DOMAIN*: ARTIFICIAL INTELLIGENCE

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTHOSH

## DESCRIPTION OF TASK
Text Summarization Using TextRank Algorithm in Python
The task implemented in the given Python script is automatic text summarization using a graph-based ranking algorithm inspired by TextRank, an adaptation of Google’s PageRank algorithm for natural language processing. Text summarization aims to create a short and meaningful summary from a longer piece of text, retaining its key points and central ideas. This is an important tool in Natural Language Processing (NLP), especially useful for summarizing news articles, research papers, documents, and more.

Overview of the Process
The script reads a text file, breaks it into sentences, calculates the similarity between every pair of sentences, and builds a similarity graph. It then applies the PageRank algorithm on this graph to rank the sentences based on their importance. Finally, it selects the top-ranked sentences to form a concise summary of the original text.

Importing Libraries:
The code uses several Python libraries: nltk for natural language processing, numpy for numerical computations, and networkx for graph-based algorithms.

Downloading Stopwords:
The nltk.corpus.stopwords are downloaded to eliminate common words like "the", "is", and "and", which do not contribute much meaning to sentence similarity.

Reading the Article:
The read_article() function opens a text file and reads its contents. The text is split into sentences, and each sentence is cleaned by removing non-alphabetic characters. Then, it splits each cleaned sentence into a list of words.

Calculating Sentence Similarity:
The sentence_similarity() function takes two sentences and calculates their cosine similarity. It builds word frequency vectors for both sentences and compares them. Cosine similarity measures how similar two sentences are based on the angle between their vector representations.

Building the Similarity Matrix:
The gen_sim_matrix() function constructs a square matrix where each cell (i, j) represents the similarity between sentence i and sentence j. This matrix acts as the weighted adjacency matrix of a graph.

Applying PageRank:
Using the networkx library, a graph is created from the similarity matrix. Then, the PageRank algorithm is applied to score each sentence. Sentences that are similar to many other important sentences get higher scores.

Generating the Summary:
The generate_summary() function sorts the sentences based on their PageRank scores and selects the top N (default is 5) to be part of the summary. These sentences are then joined and displayed as the final summary.

Applications and Significance
This method of summarization is unsupervised, meaning it does not require any training data or labeled examples. It can be used on any textual data, making it highly versatile and effective. It's especially helpful in areas like content curation, document indexing, and information retrieval. The implementation is a practical example of how NLP and graph theory can be combined to extract meaningful insights from raw text. It demonstrates the use of sentence tokenization, word embeddings (through simple frequency vectors), and graph-based ranking to solve a real-world problem in an elegant and interpretable way.

#OUTPUT

![Image](https://github.com/user-attachments/assets/369bc1af-5a8b-4bde-975a-1bf1107fbe1d)

