#  Ananya (102303160)

#  Comparative Performance Study of Clustering Algorithms

##  Project Overview

This project analyzes the performance of different clustering algorithms using various preprocessing techniques and different numbers of clusters. The goal is to evaluate how preprocessing impacts clustering quality based on multiple evaluation metrics.

##  Objectives

* Apply clustering algorithms on a real dataset (UCI Iris Dataset)
* Compare results using different preprocessing techniques
* Analyze performance across multiple evaluation metrics
* Visualize results using graphs and tables

##  Dataset

* **Dataset Used:** Iris Dataset (UCI Machine Learning Repository)
* Features: Sepal Length, Sepal Width, Petal Length, Petal Width

##  Algorithms Used

* K-Means Clustering
* Hierarchical (Agglomerative) Clustering
* Mean Shift Clustering

##  Preprocessing Techniques

* No Preprocessing
* Normalization (StandardScaler)
* PCA (Dimensionality Reduction)
* Normalization + PCA

##  Evaluation Metrics

* **Silhouette Score** → Higher is better
* **Calinski-Harabasz Index** → Higher is better
* **Davies-Bouldin Index** → Lower is better

##  Experiment Setup

* Number of clusters tested: **3, 4, 5**
* Each algorithm was evaluated with all preprocessing techniques


##  Sample Result Visualization

### Silhouette Score - Hierarchical Clustering

![Silhouette Graph]
<img width="776" height="296" alt="image" src="https://github.com/user-attachments/assets/15270df6-ffa7-4934-af0b-b0441af9b5b7" />

##  Key Observations

* PCA generally improves clustering performance in Hierarchical clustering
* Normalization alone sometimes reduces performance
* K-Means performs consistently well for structured datasets
* Mean Shift does not require specifying cluster count but is computationally expensive
* Increasing cluster count can reduce silhouette score (over-segmentation)


## Conclusion

Preprocessing plays a critical role in clustering performance. Among all methods:

* **PCA + Clustering** often gives better separation
* Choosing the correct number of clusters is essential
* No single algorithm is best — performance depends on data and preprocessing

## Tech Stack

* Python
* Scikit-learn
* Pandas
* Matplotlib

## Project Structure

```
├── clustering.ipynb
├── clustering_results.csv
├── images/
│   └── hierarchical.png
└── README.md
```

## How to Run

1. Open Google Colab / Jupyter Notebook
2. Run `clustering.ipynb`
3. Results will be generated as tables and graphs
4. CSV file will be saved automatically
