---

# Word Embeddings

This project demonstrates how to visualize **pre-trained word embeddings** ([Word2Vec](https://radimrehurek.com/gensim/auto_examples/howtos/run_downloader_api.html), [GloVe](https://nlp.stanford.edu/projects/glove/)). Word embeddings capture semantic relationships between words by representing them as vectors in a high-dimensional space. The project provides tools for dimensionality reduction and 2D visualization.

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

The notebook allows loading pre-trained word embeddings.

### Steps:
1. Load pre-trained embeddings (e.g., [GloVe](https://nlp.stanford.edu/data/glove.6B.zip)).
2. Use t-SNE or PCA for reducing embedding dimensions to 2D.
3. Visualize embeddings in 2D, revealing word clusters and relationships.

### Example:

![Word Embeddings 2D](Word%20Embeddings%202D.png)

## References

- [Word2Vec Paper](https://arxiv.org/abs/1301.3781)
- [GloVe Paper](https://nlp.stanford.edu/pubs/glove.pdf)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---
