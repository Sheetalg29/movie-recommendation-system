# 🎬 Movie Recommendation System

A full-stack AI-powered Movie Recommendation System built using **FastAPI**, **Streamlit**, **Scikit-learn**, and the **TMDB API**. The application provides personalized movie recommendations using a **TF-IDF content-based filtering algorithm** while displaying rich movie information fetched from TMDB.

---

## 🚀 Live Demo

- 🎬 **Movie Recommender App:**  
  https://movie-recommender-sheetal.streamlit.app/

- ⚙️ **FastAPI Backend:**  
  https://movie-rec-api-72y3.onrender.com/

- 📖 **Swagger API Docs:**  
  https://movie-rec-api-72y3.onrender.com/docs

**Note**: The backend is hosted on Render's free tier. If the application takes 20–30 seconds to respond on the first request, the    service is waking up. Subsequent requests are fast

## 🚀 Features

- 🔍 Search movies with real-time TMDB integration
- 🎯 Content-based movie recommendations using TF-IDF
- 🎭 Genre-based movie recommendations
- 🏠 Trending movie home feed
- 📄 Detailed movie information page
- ⭐ Movie posters, ratings, genres, release dates, and overview
- ⚡ FastAPI backend with RESTful APIs
- 🎨 Interactive Streamlit frontend
- 🔒 Secure API key management using environment variables

---


## 🛠️ Tech Stack

### Frontend
- Streamlit

### Backend
- FastAPI
- Uvicorn

### Machine Learning
- Scikit-learn
- TF-IDF Vectorizer
- Cosine Similarity

### Data Processing
- Pandas
- NumPy
- SciPy

### API Integration
- TMDB API
- HTTPX
- Requests

### Environment Management
- Python Dotenv

---

## 📂 Project Structure

```
movie-recommendation/
│
├── data/
│   ├── df.pkl
│   ├── indices.pkl
│   ├── tfidf.pkl
│   └── tfidf_matrix.pkl
│
├── app.py                 # Streamlit frontend
├── main.py                # FastAPI backend
├── movies.csv
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Sheetalg29/movie-recommendation-system.git

cd movie-recommendation-system
```

### 2. Create Virtual Environment

Windows

```bash
python -m venv .venv
```

Activate

```bash
.venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

You can get your API key from:

https://developer.themoviedb.org/

---

## ▶️ Running the Backend

```bash
uvicorn main:app --reload
```

Backend runs at

```
http://127.0.0.1:8000
```

Swagger Documentation

```
http://127.0.0.1:8000/docs
```

---

## ▶️ Running the Frontend

```bash
streamlit run app.py
```

Frontend runs at

```
http://localhost:8501
```

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/` | API Status |
| GET | `/health` | Health Check |
| GET | `/home` | Trending/Home Feed |
| GET | `/tmdb/search` | Search Movies |
| GET | `/movie/id/{tmdb_id}` | Movie Details |
| GET | `/movie/search` | Search by Movie Title |
| GET | `/recommend/tfidf` | Content-Based Recommendation |
| GET | `/recommend/genre` | Genre-Based Recommendation |

---

## 🧠 Recommendation Algorithm

This project uses a **Content-Based Filtering** approach.

Workflow:

1. Movie metadata preprocessing
2. TF-IDF vectorization
3. Cosine similarity computation
4. Top-N similar movie recommendations

The recommendation engine utilizes pre-trained pickle files for efficient inference.

---

## 📈 Future Improvements

- User authentication
- Favorite movies
- Watchlist management
- Hybrid recommendation system
- Collaborative filtering
- Movie trailers
- Pagination
- Advanced filtering
- Deployment with Docker

---

## 📦 Requirements

```
FastAPI
Streamlit
Scikit-learn
Pandas
NumPy
SciPy
HTTPX
Requests
Python Dotenv
Uvicorn
```

---


## 👩‍💻 Author

**Sheetal Gupta**

B.Tech Computer Science Engineering

Interested in:
- Artificial Intelligence
- Machine Learning
- Generative AI
- Data Science
- Backend Development

LinkedIn: *https://www.linkedin.com/in/sheetalgupta26/*

GitHub: *https://github.com/Sheetalg29*

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

```
