# Movie Recommender System

## Author
**Vansh Rana**<br>
**(Machine Learning and AI)**<br>
**Email: vansh@gmail.com**

---
## Run the Notebook Interactively
Click the link below to open the **Movie Recommender** notebook in Google Colab. You can run it, use the search input, and view movie recommendations dynamically:

[Open in Colab](https://colab.research.google.com/drive/19nPswuwBgihxclV0TeHlhANhsjEb3Vug?usp=sharing](https://colab.research.google.com/drive/19nPswuwBgihxclV0TeHlhANhsjEb3Vug?usp=sharing))


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

- **Fuzzy search** for movie titles using TF-IDF and cosine similarity.
- **Collaborative filtering** based on user ratings from the MovieLens dataset.
- **Interactive widgets** for easy search and filtering by minimum rating.

Think of it as a **personal movie concierge**: type a movie you like, and it recommends similar films that other users enjoyed.

---

## Features
- Search for movies with **partial or misspelled titles**.
- View **top recommended movies** based on collaborative filtering.
- Filter recommendations by **minimum rating**.
- Interactive experience using `ipywidgets`.

---

## Dataset
This project uses the [MovieLens 100k dataset](https://grouplens.org/datasets/movielens/100k/).  

Files used in this notebook:
- `u.item` – Movie details (ID, title, genres, year)
- `u.data` – User ratings (user ID, movie ID, rating)

**Important:**  
- Dataset is **not included in this repo** due to size.  
- Place the `ml-100k` folder in Google Drive and update the path in the notebook:

```python
dataset_path = "/content/drive/MyDrive/Colab Notebooks/ml-100k/ml-100k/"
