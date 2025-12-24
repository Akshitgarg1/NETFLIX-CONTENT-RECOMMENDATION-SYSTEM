# 🎬 Netflix Content Recommendation System

A **Content-Based Recommendation System** built using **Python, NLP, and Machine Learning** techniques that suggests similar Netflix movies and TV shows based on user preferences.  
The system analyzes textual metadata such as genre, cast, director, rating, and description to generate personalized recommendations.

---

## 📌 Project Overview

With thousands of titles available on Netflix, users often struggle to discover content aligned with their interests.  
This project solves that problem by implementing a **TF-IDF + Cosine Similarity based recommendation engine** that suggests content similar to a user’s favorite title.

The recommendation logic is entirely **content-driven**, meaning it does **not rely on user ratings or collaborative filtering**, making it scalable and effective even for new users.

---

## 🚀 Features

- 📊 Uses real-world **Netflix dataset**
- 🧠 Content-based recommendation system
- 📝 Text processing using **TF-IDF Vectorization**
- 📐 Similarity measurement using **Cosine Similarity**
- 🔍 Fuzzy matching for user input using **difflib**
- 🎯 Recommends **Top 30 similar titles**
- ⚡ Efficient and easy to extend

---

## 🛠️ Tech Stack

| Category | Tools / Libraries |
|--------|------------------|
| Programming Language | Python |
| Data Handling | Pandas, NumPy |
| NLP & ML | Scikit-learn |
| Text Vectorization | TF-IDF Vectorizer |
| Similarity Measure | Cosine Similarity |
| Input Matching | difflib |
| Environment | Google Colab / Jupyter Notebook |

---

## 📂 Dataset

- **Dataset Name:** `netflix_titles.csv`
- **Source:** Kaggle (Netflix Movies and TV Shows Dataset)
- **Key Columns Used:**
  - `title`
  - `listed_in` (genres)
  - `rating`
  - `cast`
  - `director`
  - `description`
  - `type` (Movie / TV Show)

---

## ⚙️ How It Works (Workflow)

1. **Load Dataset**
2. **Select Relevant Features**
3. **Handle Missing Values**
4. **Combine Features into a Single Text Field**
5. **Convert Text to Numerical Vectors using TF-IDF**
6. **Compute Cosine Similarity Matrix**
7. **Take User Input (Content Name)**
8. **Find Closest Matching Title**
9. **Retrieve Similar Content Based on Similarity Scores**
10. **Display Top 30 Recommendations**

---

## 🧩 Algorithm Used

### 🔹 TF-IDF (Term Frequency – Inverse Document Frequency)
Transforms textual metadata into numerical vectors while reducing the importance of commonly occurring words.

### 🔹 Cosine Similarity
Measures similarity between two content vectors by calculating the cosine of the angle between them.

---

## 🖥️ Usage Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/netflix-content-recommendation-system.git
cd netflix-content-recommendation-system
```
### 2️⃣ Install Dependencies
```bash
pip install numpy pandas scikit-learn
```
### 3️⃣ Run the Project
```bash
python project.py
```
### 4️⃣ Enter Your Favorite Content
```bash
Enter your favourite Content name : Inception
```
---
### 5️⃣ Get Recommendations
The system outputs a list of top 30 similar Netflix titles.
---
### Sample Output
```bash
Content suggested for you :

1. Interstellar
2. The Matrix
3. Shutter Island
4. The Prestige
5. Inception: The Cobol Job
...
```
### 🧠 Key Learnings
- Text feature engineering for recommendation systems

- Practical application of NLP techniques

- Efficient similarity computation

- Handling real-world datasets with missing values

- Designing scalable recommendation pipelines
---

### 🔮 Future Enhancements

- Add user-based collaborative filtering

- Integrate deep learning embeddings (Word2Vec / BERT)

- Deploy as a Flask or FastAPI web application

- Add genre-based and mood-based filters

- Improve UI with React or Streamlit

