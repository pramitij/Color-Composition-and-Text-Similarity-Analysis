# Color-Composition-and-Text-Similarity-Analysis

## Task 1: Find the proportion of main colors in a picture - to practice handling images and pixels, numpy arrays, and unsupervised clustering.
>The Image Color Analyzer notebook is a Python script designed to analyze the colors present in an image using the K-Means clustering algorithm. By identifying main colors and their proportions within the image, this tool provides insights into the color composition of the input image.

### Description
- Load Image: The script loads an image file named `rgb_colours.png` into memory using the Python Imaging Library (PIL). It ensures that the image is in the RGB color mode for compatibility with subsequent analysis.

<img width="229" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/db64a691-f36c-4598-8031-3905c77fbdb7">

- Pre-processing Data: The image data is reshaped into a flat list of pixels, which is essential for clustering algorithms to operate effectively.
- Determining Optimal Number of Clusters: The script iterates through a range of cluster numbers (k values) and computes the silhouette score for each clustering. The silhouette score measures the cohesion and separation of clusters, helping to determine the optimal number of clusters. The k value corresponding to the highest silhouette score represents the optimal number of clusters for the given image.
  
<img width="574" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/a42b6d2b-36fe-4603-b7d7-792c57221fe7">

- K-Means Clustering: Using the optimal number of clusters determined in the previous step, the script performs K-Means clustering on the pixel data. Cluster centroids are identified as main colors present in the image.
- Color Proportions Calculation: The script calculates the proportion of each main color within the image by counting the number of pixels assigned to each cluster.
- Visualization: The script provides visualizations of the main colors and their proportions within the image. It displays the main colors as individual RGB values along with their corresponding proportions. Additionally, it isolates each main color in the image, allowing for a visual representation of color distribution, highlighting its presence within the image.

<img width="531" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/f9b18190-7cb0-44ee-9d8c-a301a2969eed">

## Task 2: Find the similarity between two sentences or paragraphs - to become familiar with NLP functionalities such as tokenization, stemming, and word embeddings.
>The Sentence Similarity Analyzer notebook is a Python script designed to calculate the similarity between pairs of sentences or paragraphs using word embeddings. This assignment aims to familiarize users with Natural Language Processing (NLP) functionalities such as tokenization, stemming, and word embeddings.

## Description
I demonstrated two approaches to calculating sentence similarity:

- SpaCy Model: Initially, I utilized the spaCy library to tokenize the sentences and calculate the average word vectors for each sentence. Cosine similarity is then computed between the sentence vectors to determine their similarity. However, due to limitations in accurately capturing sentence meaning, this approach may not provide satisfactory results for certain cases.
- BERT Model: To address the limitations of the spaCy model, I tried the BERT (Bidirectional Encoder Representations from Transformers) model for sentence embedding. The sentence-transformers library was used to leverage the pre-trained BERT model and compute sentence embeddings. Cosine similarity is again calculated between the sentence pairs to evaluate their similarity.

<img width="353" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/a4885ec9-cd73-4f25-9ecd-1da1a6dbd970">

## Dependencies
- NumPy: A powerful library for numerical computing in Python.
- PIL (Python Imaging Library): A library for opening, manipulating, and saving many different image file formats.
- scikit-learn: A machine learning library in Python that provides simple and efficient tools for data mining and data analysis.
- spaCy: A library for advanced Natural Language Processing in Python.
- transformers: A library for state-of-the-art Natural Language Processing using deep learning models.
- sentence-transformers: A library for computing sentence embeddings using pre-trained transformer models.

## File Structure
- `Image_Color_Analyzer.ipynb`: The Jupyter Notebook containing the script for analyzing image colors.
- `Similarity_in_words.ipynb`: The Jupyter Notebook containing the script for analyzing sentence similarity.

## Usage Instructions
- Ensure that all dependencies are installed in your Python environment.
- Open and run the notebook using Jupyter or any compatible platform.
- Follow the instructions provided within the notebook to load an image and analyze its colors.


