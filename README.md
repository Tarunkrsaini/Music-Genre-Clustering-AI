# 🎵 Music Genre Clustering AI

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)

**Intelligent Music Discovery Using Unsupervised Machine Learning**

*Automatically group songs based on audio features using K-Means Clustering*

</div>

---

## 📌 About The Project

**Music Genre Clustering AI** is an interactive web application that uses **K-Means Clustering** to automatically discover hidden patterns in music. Instead of relying on traditional genre labels, it groups songs based on their actual audio characteristics.

The app analyzes **5 key audio features**:

| Feature | Description |
|---|---|
| 🎚️ BPM | Tempo / Speed of the song |
| ⚡ Energy | Intensity and power |
| 💃 Danceability | How suitable for dancing |
| 🔊 Loudness | Overall volume level |
| 🎙️ Speechiness | Presence of spoken words |

---

## 🚀 Features

- 🏠 **Home Dashboard** — Overview of the dataset and ML pipeline
- 📂 **Dataset Explorer** — Search and browse all songs with filters
- 🤖 **Interactive Clustering Lab** — Choose K (2–10) and run K-Means live
- 📊 **Analytics Dashboard** — Genre charts, Energy vs Danceability, BPM distribution
- 🧠 **PCA Visualization** — High-dimensional data in 2D interactive scatter plot
- 🎧 **Similar Song Finder** — AI-powered recommendations using Cosine Similarity
- 📈 **Cluster Evaluation** — Silhouette Score & Inertia metrics

---

## ⚙️ Machine Learning Pipeline

```
📁 Spotify Dataset (CSV)
        ↓
🔍 Audio Feature Selection (BPM, Energy, Danceability, Loudness, Speechiness)
        ↓
📏 Feature Scaling (StandardScaler)
        ↓
🤖 K-Means Clustering
        ↓
📊 Silhouette Score Evaluation
        ↓
🧠 PCA Dimensionality Reduction (2D Visualization)
        ↓
🎧 Similar Song Discovery (Cosine Similarity)
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Interactive web application |
| Scikit-Learn | K-Means, PCA, StandardScaler |
| Plotly | Interactive charts & visualizations |
| Pandas | Data loading and processing |

---

## 📁 Project Structure

```
Music-Genre-Clustering-AI/
├── app.py                    # Main Streamlit application
├── requirements.txt          # Project dependencies
├── README.md                 # Project documentation
├── assets/
│   └── style.css             # Custom CSS styling
├── data/
│   └── spotify_tracks.csv    # Music dataset
└── src/
    ├── clustering.py         # K-Means clustering logic
    ├── data_preprocessing.py # Data loading & cleaning
    ├── similarity.py         # Similar songs (Cosine Similarity)
    ├── navigation.py         # Sidebar navigation
    ├── evaluation.py         # Model evaluation metrics
    └── visualization.py      # Chart generation
```

---

## 🔧 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Tarunkrsaini/Music-Genre-Clustering-AI.git
cd Music-Genre-Clustering-AI
```

### 2. Create Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # macOS/Linux
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Application
```bash
streamlit run app.py
```

---

## 📊 Results

- **Best K (Clusters):** K = 2 achieved the highest Silhouette Score
- **Algorithm:** K-Means with `random_state=42`, `n_init=10`
- **Similarity Method:** Cosine Similarity within same cluster

---

## 👨‍💻 Developer

**Tarun Kr Saini**
- GitHub: [@Tarunkrsaini](https://github.com/Tarunkrsaini)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
Made with ❤️ using Python & Machine Learning
</div>