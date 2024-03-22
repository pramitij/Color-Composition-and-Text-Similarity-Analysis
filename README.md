# Color-Composition-and-Text-Similarity-Analysis

## Task1: Find the proportion of main colors in a picture - to practice handling images and pixels, numpy arrays, and unsupervised clustering.
>The Image Color Analyzer notebook is a Python script designed to analyze the colors present in an image using the K-Means clustering algorithm. By identifying main colors and their proportions within the image, this tool provides insights into the color composition of the input image.

### Usage
- Load Image: The script loads an image file named `rgb_colours.png` into memory using the Python Imaging Library (PIL). It ensures that the image is in the RGB color mode for compatibility with subsequent analysis.
- Pre-processing Data: The image data is reshaped into a flat list of pixels, which is essential for clustering algorithms to operate effectively.
- Determining Optimal Number of Clusters: The script iterates through a range of cluster numbers (k values) and computes the silhouette score for each clustering. The silhouette score measures the cohesion and separation of clusters, helping to determine the optimal number of clusters. The k value corresponding to the highest silhouette score represents the optimal number of clusters for the given image.
- K-Means Clustering: Using the optimal number of clusters determined in the previous step, the script performs K-Means clustering on the pixel data. Cluster centroids are identified as main colors present in the image.
- Color Proportions Calculation: The script calculates the proportion of each main color within the image by counting the number of pixels assigned to each cluster.
- Visualization: The script provides visualizations of the main colors and their proportions within the image. It displays the main colors as individual RGB values along with their corresponding proportions. Additionally, it isolates each main color in the image, allowing for a visual representation of color distribution.

### Example Outputs
The notebook generates visualizations to illustrate the main colors and their proportions within the image. Each main color is displayed alongside its RGB values and proportion within the image. Additionally, the script isolates each main color, highlighting its presence within the image.

<img width="574" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/a42b6d2b-36fe-4603-b7d7-792c57221fe7">

<img width="531" alt="image" src="https://github.com/pramitij/Color-Composition-and-Text-Similarity-Analysis/assets/19503874/f9b18190-7cb0-44ee-9d8c-a301a2969eed">

## Task2: Find the similarity between two sentences or paragraphs - to become familiar with NLP functionalities such as tokenization, stemming, and word embeddings.


## Dependencies
- NumPy: A powerful library for numerical computing in Python.
- PIL (Python Imaging Library): A library for opening, manipulating, and saving many different image file formats.
- scikit-learn: A machine learning library in Python that provides simple and efficient tools for data mining and data analysis.

## File Structure
- Image_Color_Analyzer.ipynb: The Jupyter Notebook containing the script for analyzing image colors.
- rgb_colours.png: The input image file used for color analysis.

## Instructions
- Ensure that all dependencies are installed in your Python environment.
- Open and run the Image_Color_Analyzer.ipynb notebook using Jupyter or any compatible platform.
- Follow the instructions provided within the notebook to load an image and analyze its colors.


