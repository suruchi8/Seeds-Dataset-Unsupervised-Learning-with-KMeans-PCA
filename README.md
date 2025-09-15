# Seeds-Dataset-Unsupervised-Learning-with-KMeans-PCA
This project applies unsupervised learning techniques to the Seeds Dataset to group wheat kernels into clusters and visualize their separation. The workflow includes clustering using KMeans and dimensionality reduction using PCA.

📊 Dataset:
https://archive.ics.uci.edu/dataset/236/seeds
The Seeds Dataset contains 210 samples with 7 features:
Area, Perimeter, Compactness, Length, Width, Asymmetry, Groove and
Class (1 = Kama, 2 = Rosa, 3 = Canadian)

🛠️ Workflow:
1. Data Loading & Exploration:
Load dataset with pandas,
Plot pairwise scatterplots with seaborn to visualize class separation
2. KMeans Clustering:
Run KMeans with n_clusters=3,
Visualize clustering results vs. ground truth for selected features
3. Higher-Dimensional Clustering:
Apply KMeans using all 7 features,
Compare cluster assignments to true labels
4. PCA for Visualization:
Reduce feature space to 2D using PCA,
Plot PCA components colored by true labels and predicted clusters

📈 Results
1. KMeans is able to roughly separate the three wheat classes, though clusters do not perfectly align with true labels.
2. PCA visualization shows that the first two components capture most of the variance and reveal clear separation between classes.
