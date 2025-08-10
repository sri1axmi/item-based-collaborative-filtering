# 🛒 Item-Based Collaborative Filtering & Random Forest Recommendation Engine

This project builds a **hybrid recommendation system** for a groceries dataset, combining **unsupervised item-based collaborative filtering** with **supervised machine learning** (Random Forest) to generate personalized product recommendations and predict purchase likelihood.

---

## 📌 Features
- **Unsupervised Item-Based Collaborative Filtering**:
  - Cosine Similarity for item closeness
  - Pearson Correlation for linear relationship analysis
  - Colorful, smaller heatmaps for easy visualization
- **Supervised Learning**:
  - Random Forest Classifier to predict purchases
  - Model evaluation using Accuracy, Precision, and Recall
- **Optimized Processing**:
  - Data handled efficiently with Pandas & NumPy
  - ML implementation via Scikit-learn
- **20% faster** recommendation generation through preprocessing optimization

## 📂 Dataset
The dataset is sourced from **[Groceries Dataset (Kaggle)](https://www.kaggle.com/heeraldedhia/groceries-dataset)** and contains:
- `Member_number` — Customer ID
- `Date` — Purchase date
- `itemDescription` — Purchased item name
## 🛠 Project Workflow
1. **Data Loading**
   - Import data from Kaggle via `kagglehub`
2. **Preprocessing**
   - Convert `Date` to `Year`, `Month`, and `Day`
   - Drop unused columns for efficiency
3. **Similarity Computation**
   - Create an item-user matrix
   - Calculate **Cosine Similarity** and **Pearson Correlation**
   - Visualize similarity matrices with Seaborn heatmaps
4. **Supervised Learning**
   - Encode categorical features
   - Train **Random Forest Classifier**
   - Evaluate model performance
5. **Results**
   - Output similarity-based recommendations
   - Display Random Forest accuracy, precision, recall

## 📊 Performance Metrics

| Model/Method        | Accuracy | Precision | Recall |
|---------------------|----------|-----------|--------|
| Random Forest       | 0.872    | 0.868     | 0.871  |
| Cosine Similarity   | N/A      | N/A       | N/A    |
| Pearson Correlation | N/A      | N/A       | N/A    |

High accuracy shows that the supervised model predicts purchases effectively, while similarity methods enhance personalization.

