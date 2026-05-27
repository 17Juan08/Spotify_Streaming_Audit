# 🎧 Spotify Streaming Audit
### Data-Driven Framework for Premium Playlist Selection

> **Can data predict which songs deserve a spot in Spotify's premium playlists?**
>
> This project combines **SQL, Data Analytics, Machine Learning, Clustering, and Business Intelligence** to identify high-performing songs and build a recommendation framework for playlist curation.

---

## 🚀 Project Overview

Spotify's catalog contains thousands of songs, but not every track generates the same engagement.

Selecting songs based solely on intuition can lead to:

- Lower playlist performance
- Reduced listener engagement
- Missed opportunities for discovery
- Less business value

This project aims to answer a simple but powerful question:

> **Which songs should be prioritized for premium playlists based on data?**

Using a dataset of approximately **2,000 Spotify tracks**, we analyzed popularity patterns, acoustic characteristics, genres, decades, and listening trends to uncover what separates average songs from top performers.

---

## 🎯 Business Goal

Develop a recommendation framework that helps Spotify:

✅ Identify premium playlist candidates

✅ Understand which genres drive popularity

✅ Discover high-performing music segments

✅ Predict song popularity using Machine Learning

✅ Support playlist decisions with data instead of intuition

---

## 📊 Project Workflow

```mermaid
flowchart LR
    A[Business Problem] --> B[Data Cleaning]
    B --> C[Exploratory Analysis]
    C --> D[SQL Insights]
    D --> E[Regression Models]
    E --> F[K-Means Clustering]
    F --> G[Dashboard]
    G --> H[Business Recommendation]
```

---

## 🔍 Key Questions

The project focuses on answering:

### 1️⃣ Which decades generate the highest popularity?

Are classic songs outperforming modern hits?

### 2️⃣ What differentiates popular songs from unpopular ones?

Do acoustic characteristics matter?

### 3️⃣ Which genres dominate among top-performing tracks?

Can genre be used as a playlist selection criterion?

### 4️⃣ Can we predict popularity?

How much of a song's success can be explained by its attributes?

### 5️⃣ Are there hidden music segments?

Can clustering reveal meaningful listener "vibes"?

---

## 📈 Key Findings

### 🎸 Classic Decades Still Matter

The **1960s and 1970s** show strong popularity performance while maintaining significant catalog representation.

### 🔥 High-Popularity Songs Share Common Traits

Songs in the highest popularity segment tend to be:

- More energetic
- More danceable
- Louder
- More positive (higher valence)
- Less acoustic

### 🎵 Genres With Strong Premium Playlist Potential

Top-performing genres include:

- Album Rock
- Dance Pop
- Alternative Rock
- Modern Rock
- Pop

### 📉 Popularity Is Not Driven By A Single Variable

Correlation analysis revealed that no individual feature fully explains popularity.

Popularity appears to emerge from a combination of:

- Genre
- Acoustic profile
- Historical context
- Musical characteristics

This motivated the use of Machine Learning and Clustering techniques.

---

## 🛠️ Tech Stack

| Category | Tools |
|-----------|---------|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| SQL | DuckDB |
| Machine Learning | Scikit-Learn |
| Clustering | K-Means |
| Dashboard | Power BI / Tableau |
| Version Control | Git & GitHub |

---

## 📂 Dataset Overview

The dataset contains Spotify song information including:

- Song Title
- Artist
- Genre
- Year
- BPM
- Energy
- Danceability
- Loudness
- Liveness
- Valence
- Duration
- Acousticness
- Speechiness
- Popularity

### 🎯 Target Variable

```python
popularity
```

The project uses popularity as the primary metric to evaluate song performance.

---

## 🧹 Data Preparation

The data preparation phase included:

- Missing value validation
- Data quality assessment
- Outlier treatment
- Feature exploration
- Correlation analysis

### Outlier Detection Techniques

- Statistical analysis
- Isolation Forest
- Multivariate anomaly detection

The cleaned dataset was then used for SQL analysis and Machine Learning modeling.

---

## 🗄️ SQL Analytics

SQL analysis was performed using **DuckDB** to answer key business questions.

### Business Questions

1. Which decades have the highest average popularity?
2. What differentiates songs across popularity quartiles?
3. Which genres dominate the highest popularity segment?
4. Which songs are strong premium playlist candidates?

### Generated Outputs

| Output File | Description |
|------------|------------|
| sql_decade_analysis.csv | Popularity by decade |
| sql_quartile_analysis.csv | Popularity quartile comparison |
| sql_top_genres_q4.csv | Top genres in the highest quartile |
| sql_premium_candidates.csv | Premium playlist candidates |

---

## 🤖 Machine Learning

### Regression Modeling

Objective:

Predict song popularity using acoustic and catalog attributes.

Evaluation Metrics:

- RMSE
- R² Score

Models under evaluation:

- Linear Regression
- K-MEANS

---

## 🎧 Clustering Analysis

K-Means Clustering is used to identify meaningful music segments.

Expected outcomes:

- Listener-oriented music groups
- Interpretable song clusters
- Playlist diversification opportunities

Evaluation:

- Silhouette Score
- Cluster Visualization
- Segment Interpretation

Example cluster labels:

- High-Energy Party Tracks
- Classic Rock Anthems
- Chill Acoustic Sessions
- Modern Pop Hits

---

## 📊 Dashboard

The dashboard is designed to transform technical findings into business insights.

### Planned Visualizations

- Popularity by Decade
- Popularity by Genre
- Popularity Distribution
- Top Playlist Candidates
- Cluster Exploration

### Interactive Filters

- Genre
- Year
- Popularity Range

---

## 💡 Business Recommendations

Current recommendations include:

1. Use the top popularity quartile as the first screening filter.
2. Prioritize genres with proven historical performance.
3. Incorporate clustering insights to improve playlist diversity.
4. Avoid selecting songs based on a single acoustic feature.
5. Combine popularity, genre, decade, and cluster membership for stronger recommendations.

---

## 📌 Project Status

| Phase | Status |
|---------|---------|
| Business Understanding | ✅ Completed |
| Data Cleaning | ✅ Completed |
| Exploratory Data Analysis | ✅ Completed |
| SQL Analytics | ✅ Completed |
| Machine Learning | 🟡 In Progress |
| Clustering | 🟡 In Progress |
| Dashboard Development | 🟡 In Progress |
| Executive Presentation | 🔵 Pending |

---

## 👥 Team

| Team Member | Role |
|------------|---------|
| Juan David Alvarado Camacho | Data Scientist & Team Lead |
| Jefferson Torres | Data Scientist |
| José Enrique Piñango Bustamante | Data Analyst |
| Jacqueline Verónica Villagómez Rodríguez | Data Analyst |

---

## 📂 Repository Structure

```text
spotify-streaming-audit/
│
├── data/
│   ├── Spotify-2000.csv
│   └── Data_spotify.zip
│
├── notebooks/
│   └── Group4_Spotify_Streaming_Audit.ipynb
│
├── outputs/
│   ├── sql_decade_analysis.csv
│   ├── sql_quartile_analysis.csv
│   ├── sql_top_genres_q4.csv
│   └── sql_premium_candidates.csv
│
├── models/
│   └── popularity_model.joblib
│
├── dashboard/
│
├── README.md
└── requirements.txt
```

---

## 🎯 Final Deliverables

- 📊 Exploratory Data Analysis
- 🗄️ SQL Business Analytics
- 🤖 Machine Learning Model
- 🎧 Music Segmentation Framework
- 📈 Interactive Dashboard
- 📑 Executive Business Recommendation

---

## ⚠️ Limitations

- Popularity may not fully represent future streaming success.
- User behavior metrics were not available.
- Correlation does not imply causation.
- Some genres contain limited observations.
- External influences such as marketing campaigns, social media trends, and artist popularity are not included.

---

## 🚀 Next Steps

- Complete regression model comparison.
- Finalize K-Means clustering analysis.
- Integrate SQL outputs into the dashboard.
- Complete executive storytelling.
- Publish final business recommendations.

---

# 🎵 From Data to Playlists

### Transforming music curation from intuition into data-driven decision making.

This project demonstrates how **Data Analytics, SQL, Machine Learning, and Business Intelligence** can be combined to support smarter playlist selection strategies and maximize listener engagement.
