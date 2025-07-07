
# 📺 Netflix Show Clustering with K-Means

> A machine learning project to group Netflix titles based on their **genre**, **rating**, and **duration** using **K-Means Clustering** and visualize them using **Principal Component Analysis (PCA)**.

---

## 📌 Project Objective

This project uses **unsupervised learning** to explore hidden patterns in the Netflix catalog. By applying **K-Means clustering**, we group shows that share similar characteristics — helping to uncover potential content categories and insights that could power recommendation systems or content segmentation strategies.

---

## 🧰 Tech Stack

- 🐍 Python  
- 📊 Pandas & NumPy  
- 🧠 Scikit-learn  
- 📈 Seaborn & Matplotlib  
- 🔍 PCA for dimensionality reduction  
- 📁 Dataset: [Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## 🧪 Features & Workflow

### 1. **Dataset Loading & Cleaning**
- Loaded the `netflix_titles.csv` dataset
- Selected key columns: `title`, `listed_in`, `rating`, `duration`
- Filtered and transformed `duration` to numeric values (minutes only for movies)
- Simplified `genre` by extracting the primary genre
- One-hot encoded categorical variables: genre and rating

### 2. **Preprocessing**
- Normalized numerical values using `StandardScaler`
- Prepared a clean feature set for clustering

### 3. **Clustering**
- Applied **K-Means** clustering to group shows into `k=5` clusters
- Labeled each show with a cluster ID

### 4. **Dimensionality Reduction**
- Used **PCA** to reduce high-dimensional feature space to 2D for visualization
- Retained most of the data’s variance

### 5. **Visualization**
- Created a scatter plot of clusters using Seaborn
- Color-coded clusters to show how Netflix shows group based on their features

---

## 📈 Output

- 🚀 **5 distinct clusters** of Netflix shows
- 📌 Shows in each cluster share similar:
  - Primary genre
  - Viewer rating (e.g., PG, TV-MA)
  - Duration (e.g., short or long movies)
- 📉 PCA visualization highlights the effectiveness of clustering

---

## 📸 Sample Plot

![Netflix Clustering PCA](your-clustering-image-path.png)  
*Each point represents a show, colored by its cluster.*

---

## 🔍 Use Cases

- 🔁 Build a **recommendation engine** using cluster similarity
- 🎯 Targeted content curation for user personas
- 📊 Analyze trends in genres and duration across the Netflix catalog

---

## 🧠 Key Learnings

- Understanding **unsupervised learning** via K-Means
- Importance of **data preprocessing** and encoding
- Power of **PCA** for simplifying complex datasets for visualization
- Interpreting and explaining cluster behavior based on real-world media features

---

## 📁 Dataset

- 📦 **Source**: [Kaggle – Netflix Titles Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- Includes ~7,000+ entries of Movies and TV Shows with details like:
  - `Title`, `Type`, `Genre`, `Rating`, `Duration`, `Description`

---

## 📚 Future Improvements

- Use **multi-label binarization** for multiple genres
- Include **description** using **TF-IDF vectorization** for deeper content-based clustering
- Tune the number of clusters using **Elbow Method** or **Silhouette Score**

---

## 🤝 Credits

Made by **Fizzah Abdullah** | Data Science Student | Passionate about ML & Insightful Visualizations.

> For any questions or collaboration ideas, feel free to connect!
