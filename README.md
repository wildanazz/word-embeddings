---

# Word Embeddings

This project demonstrates how to visualize **pre-trained word embeddings** (Word2Vec, GloVe). Word embeddings capture semantic relationships between words by representing them as vectors in a high-dimensional space. The project provides tools for dimensionality reduction and 2D visualization.

## Prerequisites
- **Python 3.x**
- **Jupyter Notebook**
- **Gensim**
- **Matplotlib**
- **Scikit-learn**

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/wildanazz/word-embeddings.git
   cd word-embeddings
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

## Usage

The notebook allows loading pre-trained word embeddings like Word2Vec or GloVe.

### Steps:
1. Load pre-trained embeddings (e.g., Word2Vec).
2. Use t-SNE or PCA for reducing embedding dimensions to 2D.
3. Visualize embeddings in 2D, revealing word clusters and relationships.

### Example:
```python
# Load embeddings
import gensim.downloader as api
model = api.load('glove-wiki-gigaword-100')

# Perform t-SNE for 2D visualization
from sklearn.manifold import TSNE
import matplotlib.pyplot as plt
import numpy as np

words = ['king', 'queen', 'man', 'woman', 'apple', 'orange']
word_vectors = np.array([model[word] for word in words])  # Convert to NumPy array

tsne = TSNE(n_components=2, perplexity=2)
word_vectors_2d = tsne.fit_transform(word_vectors)

# Plot the 2D representation
plt.figure(figsize=(10, 10))
for i, word in enumerate(words):
    plt.scatter(word_vectors_2d[i][0], word_vectors_2d[i][1])
    plt.text(word_vectors_2d[i][0] + 0.05, word_vectors_2d[i][1] + 0.05, word, fontsize=12)
plt.show()
```
![Word Embeddings 2D](Word%20Embeddings%202D.png)

## References

- [Word2Vec Paper](https://arxiv.org/abs/1301.3781)
- [GloVe Paper](https://nlp.stanford.edu/pubs/glove.pdf)

---
