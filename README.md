# customer-segmentation-mall

## Project Description

This project focuses on customer segmentation based on the **Mall Customers** dataset. The objective is to group customers into different clusters according to their behaviors and spending patterns, providing insights for marketing strategies and customer relationship management.

## Project Structure

- `clustering_mall_customer.ipynb`: Jupyter notebook performing data preprocessing, clustering with KMeans, and evaluation.
- `mall_customers.csv`: Raw customer dataset.
- `kmeans_clustering_result.csv`: Output file containing each customer's assigned cluster.
- `mall_customer_dashboard.pbix`: Power BI dashboard for visualizing and analyzing the clustering results.

## Steps Performed

### Data Preprocessing

- Encoded the categorical `Genre` column using Label Encoding.

### Feature Selection

- Selected the following features for clustering: `Genre`, `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`.

### Finding Optimal Number of Clusters

- Applied the Elbow method to determine the best number of clusters.

### Modeling

- Built a KMeans clustering model with the optimal number of clusters.

### Evaluation

- Evaluated the model using Silhouette Score, Davies-Bouldin Score, and Calinski-Harabasz Score.

### Visualization

- Reduced data dimensions using PCA and visualized clusters with a scatter plot.

### Result Export and Dashboard Design

- Exported the clustering results to a CSV file.
- Designed a dashboard in Power BI to interpret customer segments visually.

## Technologies Used

- Python (pandas, scikit-learn, matplotlib, seaborn, yellowbrick)
- Power BI

## How to Run the Project

1. Open and run the `clustering_mall_customer.ipynb` notebook to perform clustering and generate the `kmeans_clustering_result.csv` file.
2. Open the `mall_customer_dashboard.pbix` file in Power BI Desktop to explore and analyze the dashboard.

> Note: The raw dataset (`mall_customers.csv`) is included in the project.

## Environment Setup

Install the required Python libraries with the following command:

```bash
pip install pandas scikit-learn matplotlib seaborn yellowbrick
