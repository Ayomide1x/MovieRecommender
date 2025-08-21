# Movie Recommendation Engine


Ever wondered how Netflix or Google suggests movies similar to the ones you like? This repository demonstrates how to build a **Movie Recommendation System** using different techniques, including **Popularity-Based**, **Content-Based**, and **Collaborative Filtering** approaches.  

In this repository, we implement a **Content-Based Recommendation Engine** using the **Scikit-Learn** library. It shows how to compute movie similarities based on features like cast, director, genres, and keywords to recommend movies tailored to user preferences.

---

## 🚀 Features

1. **Types of Recommendation Engines Explained**
   -  **Popularity-Based**: Suggests trending or most-watched movies (e.g., YouTube trending list).
   -  **Content-Based**: Recommends movies similar to a given movie by analyzing its features (cast, director, genres, etc.).
   -  **Collaborative Filtering**: Suggests movies based on similar users’ viewing history (e.g., “Customers who watched this also watched”).
   -  **Hybrid Systems**: Combination of two or more techniques.

2. **Content-Based Recommendation Engine Implementation**
   - Extracts movie features such as cast, director, genres, and keywords.
   - Uses **CountVectorizer** and **Cosine Similarity** to find and rank similar movies.
   - Returns the **Top-N most similar movies** to a user-selected movie.

3. **Advanced Ranking**
   - Ranks recommended movies not only by similarity but also by **average user ratings** for higher quality suggestions.

---

## 📊 How It Works

1. **Preprocessing the Dataset**
   - Combines selected features (cast, director, genres, keywords) into a single text field.
   - Converts text into numerical vectors using `CountVectorizer`.

2. **Computing Similarity**
   - Applies `cosine_similarity` to measure how close two movies are.
   - Generates a similarity matrix for all movies.

3. **Making Recommendations**
   - Retrieves the most similar movies to a user-given movie.
   - Sorts recommendations by similarity score and/or rating.

---

## 🛠️ Dependencies

- **pandas** : For dataset handling.  
- **numpy** : For numerical operations.  
- **scikit-learn** : For vectorization and cosine similarity.  

Install all dependencies with:
```bash
pip install pandas numpy scikit-learn
```
