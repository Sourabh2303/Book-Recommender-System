# 📚 Book Recommender System

This is a Flask-based web application that recommends books based on a selected title. It uses collaborative filtering and precomputed similarity scores to suggest books that are most similar to the one chosen by the user.

![App Preview](https://book-recommender-system-gak9.onrender.com) <!-- Optional: Add a screenshot or demo gif -->

---

## 🚀 Features

- 🔍 Recommend similar books using collaborative filtering
- 📊 Preprocessed data for fast recommendations
- 📚 Top 50 most popular books shown on the homepage
- 🌐 Responsive UI with Bootstrap 5
- 🧠 Model files loaded from pickle format (`.pkl`)
- 🖥️ Deployable on Render.com or any cloud platform

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, Bootstrap
- **Backend:** Python, Flask
- **Model:** Collaborative filtering using cosine similarity
- **Deployment:** Render

---

Book-Recommender-System/
│
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── Procfile               # Deployment file for Render
├── popular.pkl            # Top 50 books data
├── books.pkl              # Books metadata
├── pt.pkl                 # Pivot table for similarity
├── similarity_score.pkl   # Precomputed similarity scores
│
└── templates/             # HTML templates
    ├── index.html         # Homepage
    └── recommend.html     # Recommendation UI


---

## 🧪 How It Works

- The user selects a book from a dropdown.
- The app finds similar books using cosine similarity on a pivot matrix.
- Recommended books (title, author, cover image) are shown instantly.

---

## 💻 Setup Locally

1. **Clone the repo:**
   ```bash
   git clone https://github.com/Sourabh2303/Book-Recommender-System.git
   cd Book-Recommender-System
Create a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the app:

bash
Copy code
python app.py
Open your browser at http://127.0.0.1:5000

☁️ Deploy on Render
Create a free account at https://render.com

Connect your GitHub repo

Add a new Web Service with the following settings:

Build Command: pip install -r requirements.txt

Start Command: gunicorn app:app

Add a Procfile with:

bash
Copy code
web: gunicorn app:app

🧑‍💻 Author
Sourabh Kumar




