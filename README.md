
# Movie Recommender System

This is a **content-based movie recommender system** built using **Python**, **Streamlit**, and **scikit-learn**. It suggests similar movies based on the one you select, using cosine similarity on movie metadata features.

---

## 🚀 Features

- Recommend top 5 movies similar to a selected movie
- Movie posters fetched via [TMDb API](https://www.themoviedb.org/documentation/api)
- Clean and interactive UI with Streamlit
- Lightweight and easy to deploy

---

## 📦 Tech Stack

- Python 3.8+
- Streamlit
- Pandas
- Scikit-learn
- Requests
- Pickle (for precomputed similarity & movie data)

  ---
##  Dataset
The Movie Database (TMDb) in accordance with their terms of use. 

Download the (Dataset)[https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata]
---

## 🖥️ Live Demo

> _Coming soon on Streamlit Cloud or Render!_

---

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender
````

### 2. Create a Virtual Environment (optional)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Add Your TMDb API Key

Create a file called `.env` (or update directly in the code):

```
TMDB_API_KEY=your_api_key_here
```

Or edit this line in `app.py`:

```python
url = f"https://api.themoviedb.org/3/movie/{movie_id}?api_key=YOUR_KEY&language=en-US"
```

### 5. Run the App

```bash
streamlit run app.py
```

---

## 📁 Folder Structure

```
├── app.py                      # Main Streamlit app
├── Model/
│   ├── movie_list.pkl          # Movie metadata
│   ├── similarity.pkl          # Precomputed similarity matrix
├── requirements.txt
└── README.md
```

---

## 📌 How It Works

1. Load movie metadata and similarity matrix
2. Select a movie from the dropdown
3. Recommend top 5 similar movies based on cosine similarity
4. Fetch and display posters via TMDb API

---

## 💡 Future Improvements

* Include genre and rating filters
* Add collaborative filtering model
* Deploy on Streamlit Cloud or Render

---

## 📜 License

MIT License. Free to use and modify.

---

## 🤝 Contributing

Feel free to fork this repo, open issues, or submit pull requests.


