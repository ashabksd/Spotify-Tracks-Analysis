# 🎧 Spotify Tracks Exploratory Data Analysis

An in-depth exploratory data analysis (EDA) of over 2,000 Spotify tracks to uncover trends, correlations, and insights from the world of digital music.

---

## 📌 Introduction

The "Spotify Tracks Analysis" project explores and visualizes a dataset containing metadata and audio features for various Spotify songs. The main goal is to gain insights into song characteristics, identify patterns, and understand correlations using Python and libraries like Pandas, NumPy, Matplotlib, and Seaborn.

---

## 🧼 Data Loading and Cleaning

- The dataset is loaded using `pandas` from a CSV file.
- Columns include: `id`, `name`, `popularity`, `duration_ms`, `artists`, `release_date`, and various audio features like `energy`, `loudness`, `acousticness`, etc.
- Initial checks for missing values using `isnull()` and `.info()`

---

## 🔍 Exploratory Data Analysis

### 🎵 1. 10 Least Popular Songs
Tracks are sorted in ascending order by popularity to reveal the least popular songs in the dataset.

### 🌟 2. 10 Popular Songs with Popularity > 90
Highlights the most popular songs with a popularity score greater than 90.

---

## 🔄 Data Transformation

- The duration of songs (initially in milliseconds) is converted to **seconds**.
- `duration_ms` is dropped.
- New column `duration` is added for clarity.

---

## 📊 Visualizations

### 🔥 Correlation Heatmap

Shows how audio features relate to one another (after removing non-numeric or categorical features like `key`, `mode`, and `explicit`).

![Correlation Heatmap](images/correlation_heatmap.png)

---

### 🎚️ Regression Plots

#### 1. Loudness vs Energy
Visualizes how louder songs tend to be more energetic.

![Loudness vs Energy](images/loudness_vs_energy.png)

#### 2. Popularity vs Acousticness
Reveals whether acoustic songs are more or less popular.

![Popularity vs Acousticness](images/popularity_vs_acousticness.png)

---

## ✅ Conclusion

The "Spotify Tracks Analysis" project successfully explores key audio and popularity features of Spotify songs. Using EDA and data visualization, we uncovered:

- Positive correlation between energy and loudness
- Noisy but insightful trends between popularity and acousticness
- A shift in song durations across years

These insights reflect evolving listener preferences and production trends in the music industry.

---



