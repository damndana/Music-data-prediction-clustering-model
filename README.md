# 🎶 Music Data Prediction & Clustering Model 🎧  
Predicting moods & mapping musical vibes using Apple Music Wrapped + Machine Learning

---

## 🧠 Project Summary

This project combines **machine learning** and **personal listening data** to explore how music reflects and influences mood across time. Using my **January–June Apple Music Wrapped stats**, I:

- 📈 **Predicted** my musical mood for the upcoming month using **Linear Regression**
- 🎨 **Clustered** my top artists into distinct **mood groups** with **K-Means Clustering**
- 💾 Created and processed my own dataset from scratch in CSV format

The result? A beautiful, data-driven reflection of my emotional journey through music — and a model that adapts with every listen 💫

---

## 💽 Dataset

- Custom-made `apple_music_mood.csv` file
- Fields include:
  - `Month`
  - `Top Artists`
  - `Top Songs`
  - `Minutes Listened`
  - `Energy`, `Valence`, `Tempo` (derived via Spotify API or estimated manually)
  - `Dominant Mood` (labeled per month — e.g., "Chill", "Hype", "Melancholy")

---

## ⚙️ Tech Stack & Tools

- `Python`
- `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
- `Scikit-learn`: LinearRegression, KMeans, Silhouette Score
- `Jupyter Notebook` for experimentation
- CSV + manual preprocessing

---

## 🔍 Machine Learning Breakdown

### 🧪 1. **Linear Regression**
- Used to predict **next month's music mood** based on:
  - Past mood scores
  - Listening time
  - Audio features (valence, energy, tempo)
- Evaluated using `MAE`, `R² Score`

### 🎯 2. **K-Means Clustering**
- Grouped top artists into **mood clusters**:
  - e.g., "Energetic", "Melancholic", "Feel-Good"
- Visualized using:
  - Elbow Method
  - 2D PCA plots
  - Silhouette Scores for cluster validation
