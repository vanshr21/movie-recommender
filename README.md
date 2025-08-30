# Movie Recommender System

**Author:** Vansh Rana (Machine Learning & AI)  
**Email:** vansh@gmail.com

---

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://colab.research.google.com/drive/19nPswuwBgihxclV0TeHlhANhsjEb3Vug?usp=sharing](https://colab.research.google.com/github/vanshr21/movie-recommender/blob/main/Movie_Recommendation_System.ipynb
)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

> **Note:** The notebook is read-only when opened via the link above. To experiment, save a copy to your own Google Drive (**File → Save a copy in Drive**).

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Dataset](#dataset)
4. [Installation & Setup](#installation--setup)
5. [How to Run](#how-to-run)
6. [Notes](#notes)
7. [License](#license)

---

## Project Overview
This repository contains a **Movie Recommendation System** implemented in Python.  
It allows users to search for movies and get personalized recommendations based on:

- **Fuzzy search** for movie titles using TF-IDF and cosine similarity
- **Collaborative filtering** based on user ratings from the MovieLens dataset
- **Interactive widgets** for easy search and filtering by minimum rating

Think of it as a **personal movie concierge**: type a movie you like, and it recommends similar films that other users with similar tastes enjoyed.

---

## Features
- **Interactive Movie Search**: Find movies using a fuzzy text search.
- **Dynamic Recommendations**: Use a slider to set a minimum rating threshold for recommendations.
- **Easy to Use**: Built with Pandas, Numpy, and Scikit-learn.
- **Colab Ready**: Fully interactive in Google Colab.

---

## Dataset
This project uses the **MovieLens 100k dataset** from [GroupLens](https://grouplens.org/datasets/movielens/100k/).

**Files used:**
- `u.item` – Movie details (ID, title, genres, year)
- `u.data` – User ratings (user ID, movie ID, rating)

**Important:**  
- Dataset is **not included** in this repository.  
- Place the `ml-100k` folder in Google Drive, ideally inside `/Colab Notebooks/`.  
- Update the dataset path in the notebook:

```python
dataset_path = "/content/drive/MyDrive/Colab Notebooks/ml-100k/"
```

---

## Installation & Setup

### Local Setup (Optional)
1. **Clone the repository:**
```bash
git clone https://github.com/<your-username>/Movie_Recommender.git
```
2. **Install required libraries:**
```bash
pip install pandas numpy scikit-learn ipywidgets
```

### Google Colab Setup (Recommended)
1. **Upload the Dataset**: Place the `ml-100k` folder in your Google Drive.  
2. **Open the Notebook**: Open the `.ipynb` file in Google Colab.

---

## How to Run
1. **Mount Google Drive** (if using Colab):
```python
from google.colab import drive
drive.mount('/content/drive')
```
2. **Update Dataset Path** in the notebook:
```python
dataset_path = "/content/drive/MyDrive/Colab Notebooks/ml-100k/"
```
3. **Run All Cells** via **Runtime → Run all**.  
4. **Get Recommendations** using the movie search input and the minimum rating slider.  
5. **Save Your Work**: Use **File → Save a copy in Drive** to make changes safely.

---

## Notes
- The notebook is **read-only** via the shared Colab link. Save a copy to edit.  
- Widgets are interactive only in Colab/Jupyter; GitHub shows a static preview.  
- Ensure the MovieLens dataset is correctly placed; otherwise, the notebook won’t load.

---

## License
This project is released under the **MIT License**.  
You may use, modify, and distribute the code for educational and personal purposes.
