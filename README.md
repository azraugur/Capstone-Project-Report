# 🎬 Netflix-style Movie Recommendation System

## 📌 Project Overview

This project builds a **personalized movie recommendation system** inspired by Netflix.  
Due to the rapid growth of OTT platforms, users experience information overload and difficulty choosing content.  

To solve this problem, we develop a **hybrid recommendation system** using machine learning techniques.

---

## ❗ Problem Statement

- Too many contents in OTT platforms  
- User decision fatigue  
- Poor personalization in traditional recommendation systems  
- Limited use of user behavior data  

---

## 💡 Proposed Solution

We propose a **Hybrid Recommendation System** that combines:

- Collaborative Filtering (user behavior-based)
- Content-Based Filtering (movie feature-based)
- Machine Learning prediction model

📌 Future improvement:
- LLM-based explanation system for recommendations

---

## 📊 Dataset

We use the **MovieLens Dataset**.

👉 Dataset source: https://grouplens.org/datasets/movielens/

### 📁 MovieLens 1M Statistics:
- ⭐ 1,000,209 ratings  
- 👤 6,000 users  
- 🎬 4,000 movies  

### 📂 Files:

- `ratings.dat` → userId, movieId, rating, timestamp  
- `movies.dat` → movieId, title, genres  
- `users.dat` → user information (optional)

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handling missing values  
- Data normalization  
- Encoding categorical variables  

---

### 2. Feature Engineering
- Movie genre extraction  
- User-item matrix creation  
- TF-IDF / vectorization for content features  

---

### 3. Recommendation Models

#### 🔹 Collaborative Filtering
- User similarity computation  
- User-item interaction matrix  

#### 🔹 Content-Based Filtering
- Cosine similarity between movie features  

#### 🔹 Hybrid Model

```python
final_score = 0.5 * collaborative_score + 0.5 * content_score
