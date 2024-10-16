# Customer Segmentation using KMeans Clustering

This project demonstrates customer segmentation using the KMeans clustering algorithm. The goal is to categorize customers into distinct segments based on their annual income and spending scores. These insights can help businesses target customers more effectively by creating tailored marketing strategies for each segment.

## Project Overview

Customer segmentation is a crucial part of understanding customer behavior and preferences. By clustering customers based on key features like annual income and spending habits, businesses can:
- Identify high-value customers
- Target low-income customers with specific offers
- Improve personalized marketing strategies
- Understand the diverse spending behaviors of their customer base

This project implements the KMeans algorithm for customer segmentation, visualizes the clusters, and provides actionable insights.

## Dataset

The dataset used for this project is the [Mall Customer Segmentation Data](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python). It contains the following columns:
- **CustomerID**: Unique ID for each customer
- **Gender**: Gender of the customer
- **Age**: Age of the customer
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars
- **Spending Score (1-100)**: Score assigned by the mall based on customer spending behavior

## Project Steps

1. **Data Preprocessing**:
    - Loaded the dataset and performed initial data cleaning.
    - Dropped unnecessary columns such as `CustomerID` and `Gender` (if not needed for clustering).
    - Standardized the dataset for better clustering results.

2. **KMeans Clustering**:
    - Applied the KMeans algorithm to group customers into segments.
    - Chose the optimal number of clusters using the Elbow method.
    - Visualized the clusters using a scatter plot.

3. **Model Prediction**:
    - Once the model was trained, predictions were made for new customer data.
    - The model returns the segment the customer belongs to, which can guide personalized marketing.

4. **Visualization**:
    - Visualized the customer clusters using `matplotlib` and `seaborn` libraries.
    - Generated a scatter plot to display clusters based on annual income and spending score.

## How to Run the Project

### Prerequisites

Make sure you have the following installed:
- Python 3.x
- Jupyter Notebook or Google Colab (if running interactively)
- Libraries:
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `seaborn`
    - `sklearn`

### Steps to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/customer-segmentation.git
    cd customer-segmentation
    ```

2. Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

3. Run the Jupyter notebook or Python script to execute the clustering algorithm and generate the output:
    ```bash
    jupyter notebook customer_segmentation.ipynb
    ```

4. Use the model to predict the cluster of new customers by passing their annual income and spending score to the `predict` function.

## Key Insights from the Project

- Identified four distinct customer segments:
    - High-income, high-spending customers
    - High-income, low-spending customers
    - Low-income, high-spending customers
    - Low-income, low-spending customers
- Provided actionable insights for targeted marketing and customer retention strategies.

## Future Work

- Add additional features like customer age, gender, and geographical location for a more comprehensive segmentation model.
- Implement other clustering algorithms (e.g., hierarchical clustering, DBSCAN) for comparison.
- Build a recommendation engine based on customer segments to suggest products.

## Repository Structure

```bash
customer-segmentation/
│
├── dataset/
│   └── Mall_Customers.csv         # Dataset used for clustering
│
├── customer_segmentation.ipynb    # Jupyter notebook for the project
│
├── customer_segmentation.py       # Python script for the project
│
└── README.md                      # Project README file
