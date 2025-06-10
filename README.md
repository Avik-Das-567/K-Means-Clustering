# K-Means Clustering
### App Link
- https://k-means-clustering-1.streamlit.app/
---
### What is K-Means Clustering?
- K-Means is an **unsupervised machine learning algorithm**.
- It groups **similar data points** together into **K clusters**.
- We just tell the machine: "**Make K groups**", and it figures out the best way.
- **Example:** We want to arrange students into **3 study groups** based on their marks in Math and Science. K-Means will group similar students together based on scores.
---
### Required Python Packages
- **`scikit-learn`** - To build machine learning models
- **`streamlit`** - To build data apps
- **`pandas`** - To work with the dataset
- **`matplotlib`** - To plot the clustered data visually
---
### Example Problem
- **Input Data:**

| X (Math Marks) | Y (Science Marks) |
| -------------- | ----------------- |
| 1              | 2                 |
| 2              | 3                 |
| 8              | 8                 |
| 9              | 10                |
| 10             | 11                |
| 25             | 30                |

- We want to **group them into 3 clusters**.
---
### How It Works
- Choose how many groups we want (**K**).
- It places **K** points (centers).
- Assigns each data point to the **nearest center**.
- Moves the center to the **middle of the group**.
- Repeats until it stabilizes.
---
### Expected Output Table

| X  | Y  | Cluster |
| -- | -- | ------- |
| 1  | 2  | 2       |
| 2  | 3  | 2       |
| 8  | 8  | 0       |
| 9  | 10 | 0       |
| 10 | 11 | 0       |
| 25 | 30 | 1       |

- Group 0: **Middle Scorers**
- Group 1: **High Scorers**
- Group 2: **Low Scorers**
---
### Additional Insights :
- K-Means doesn't use any labels. It just looks at **similarity**.
- We have to decide the **K (number of groups)** ourselves.
- The algorithm may give **slightly different results** each time (random start).
---
