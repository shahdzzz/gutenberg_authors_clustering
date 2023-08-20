# Project: Gutenberg Authors Clustering using Text Features

This project aims to cluster a collection of books from Project Gutenberg based on their textual content using various text representation techniques and clustering algorithms. The goal is to explore how different clustering methods perform in grouping books from different genres written by distinct authors. The project utilizes a diverse set of books spanning multiple genres, including Detective and Mystery Fiction, Biography, Horror, Romance, and Classic literature.

## Dataset

The dataset consists of five books, each from a different genre:

1. **The Adventures of Sherlock Holmes**
   - Author: Arthur Conan Doyle
   - Genre: Detective and Mystery Fiction
   - [Download Link](https://www.gutenberg.org/files/1661/1661-0.txt)

2. **Queen Victoria**
   - Author: Lytton Strachey
   - Genre: Biography
   - [Download Link](https://www.gutenberg.org/cache/epub/1265/pg1265.txt)

3. **Dracula**
   - Author: Bram Stoker
   - Genre: Horror
   - [Download Link](https://www.gutenberg.org/cache/epub/345/pg345.txt)

4. **Pride and Prejudice**
   - Author: Jane Austen
   - Genre: Romance
   - [Download Link](https://www.gutenberg.org/cache/epub/1342/pg1342.txt)

5. **The Great Gatsby**
   - Author: F. Scott Fitzgerald
   - Genre: Classic
   - [Download Link](https://www.gutenberg.org/files/64317/64317-0.txt)

## Preprocessing

The following preprocessing steps are applied to the text of each book:
1. Removal of stop words
2. Lemmatization of words
3. Removal of punctuation

## Text Representation Techniques

The following text representation techniques are used to transform the preprocessed text into numerical features:

1. Bag of Words (BoW)
2. Term Frequency-Inverse Document Frequency (TF-IDF)
3. Word2Vec
4. Doc2Vec
5. FastText
6. BERT embeddings

## Clustering Algorithms

The following clustering algorithms are applied to the text features:

1. K-Means
2. Expectation Maximization (EM)
3. Agglomerative Clustering

## Model Evaluation

For each clustering model, the following evaluation metrics are computed:

1. Silhouette Score: Measures the quality of the clusters formed.
2. Kappa Score: Measures the agreement between predicted clusters and true labels.

## Determining Optimal Clusters

The Elbow Method is used to determine the optimal number of clusters for each model. This involves plotting the within-cluster sum of squares (WCSS) against the number of clusters and identifying the "elbow point" where the rate of decrease changes.

## Error Analysis

Cosine similarity is used to compare the similarity between the true genre labels and the predicted cluster labels. This analysis helps us understand how well the clustering algorithm has captured the inherent structure of the data and if there are any discrepancies between true and predicted labels.

## Usage

1. Download the required books using the provided links.
2. Preprocess the text using the specified preprocessing steps.
3. Transform the text into numerical features using the mentioned text representation techniques.
4. Apply different clustering algorithms to the features.
5. Evaluate the performance of each model using silhouette and kappa scores.
6. Determine the optimal number of clusters using the Elbow Method.
7. Perform error analysis using cosine similarity to compare true and predicted labels.

## Conclusion

This project showcases the application of various text representation techniques and clustering algorithms to group books from different genres based on their textual content. The evaluation metrics and error analysis provide insights into the effectiveness of different models in capturing the underlying patterns in the data. By experimenting with different techniques and algorithms, we can gain a deeper understanding of how text clustering can be used to organize and analyze diverse literary works.
