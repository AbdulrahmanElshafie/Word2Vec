# Natural Language Processing Text Embedding Pipeline - Word2Vec
This project demonstrates a natural language processing (NLP) pipeline for text embedding and similarity analysis. It leverages the NLTK library for preprocessing and the Gensim library for word embedding generation.

## Code Structure
The code is organized into the following key steps:

### 1. Data Preparation:
- Reads the document from a CSV file (embedding_task.csv).
- Converts the document to a string representation.

### 2. Text Preprocessing:
- `text_preprocessing` function:
- Lowercases text.
- Removes punctuation.
- Removes stop words using NLTK's stopword list.
- Lemmatizes words using NLTK's WordNetLemmatizer to handle morphological variations.

### 3. Tokenization and Word2Vec Training:
- Tokenizes each preprocessed text into individual words using NLTK's word_tokenize.
- Trains a Word2Vec model using Gensim's Word2Vec class, capturing semantic relationships between words.
- Explores the resulting word embeddings.

### 4. Similarity Measures:
- Calculates cosine similarity, Jaccard similarity, and Euclidean distances between word embeddings to assess their semantic closeness.
- Creates heatmaps using Seaborn to visualize the similarity matrices.

### 5. Dimensionality Reduction with MDS:
- Performs Multidimensional Scaling (MDS) to project the high-dimensional similarity matrices into a 2D space for better visualization.
- Creates scatter plots with annotations for each sentence, allowing for easier interpretation of semantic relationships.
