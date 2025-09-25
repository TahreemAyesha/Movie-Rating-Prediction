# Movie-Rating-Prediction
# 🎬 Movie Rating Prediction with SVD

## 📌 project Overview
This project builds a **movie rating prediction** using the **Surprise library** in Python.  
We apply **Singular Value Decomposition (SVD)**, a collaborative filtering algorithm, to predict how a user would rate unseen movies.

---

## 📂 Dataset
  
- **Columns used:**
  - `userId`  
  - `movieId`   
  - `rating`  
  



## ⚙️ Steps
1. Import libraries (`pandas`, `surprise`)  
2. Load dataset and select columns  
3. Convert into Surprise format (`Dataset.load_from_df`)  
4. Split into train/test sets (80/20)  
5. Train SVD model  
6. Make predictions  
7. Evaluate with **RMSE** and **MAE**  



## 📊 Results
- **RMSE:** `1.4664`  
- **MAE:** `1.2658`  

---

## 🔎 Interpretation
The model performs reasonably well, showing that SVD can learn meaningful patterns in user–movie interactions.  
On average, predictions are within **1.3 stars of the true rating**, which is a good baseline for recommendation tasks on such a large and sparse dataset.  
The results also highlight a common trend in collaborative filtering: the model tends to predict ratings closer to the middle (around 3 stars), leading to some overestimation of low ratings and underestimation of high ratings.  

 
