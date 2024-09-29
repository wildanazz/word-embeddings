---

# Word Embeddings

This project explores word embeddings and visualizes them in a 2D space using machine learning techniques like Word2Vec or GloVe. Word embeddings are vector representations of words, capturing semantic meaning based on their usage in text data.

## Features
- **Word Embedding Generation**: Create high-dimensional vector representations of words.
- **2D Visualization**: Project word vectors into two dimensions for visualization.
- **Jupyter Notebook**: The entire process is executed and demonstrated within a Jupyter notebook.

## Prerequisites

- **Python 3.x**
- **Jupyter Notebook**
- **Matplotlib**: For visualization.
- **Scikit-learn**: For dimensionality reduction (PCA or t-SNE).
- **Gensim**: For generating word embeddings using models like Word2Vec.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/wildanazz/word-embeddings.git
   cd word-embeddings
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

## Usage

The project provides an interactive Jupyter notebook (`main.ipynb`) where you can visualize word embeddings.
  
### Dimensionality Reduction and Visualization

- The high-dimensional word vectors are reduced to two dimensions using techniques like PCA or t-SNE, allowing for 2D visualization of semantic word relationships.
- You can visualize the embeddings and explore how similar words cluster together.

## Example

- Visualize the 2D embeddings:
  ![Word Embeddings 2D](Word%20Embeddings%202D.png)

## Customization

- You can also experiment with different dimensionality reduction techniques (e.g., PCA vs. t-SNE).

## References

- [Word2Vec Paper](https://arxiv.org/abs/1301.3781)
- [GloVe Paper](https://nlp.stanford.edu/pubs/glove.pdf)

---
