#Movie Recommender System

Movie Recommender System

A simple content-based movie recommender built with Python. Enter a movie title, get a list of similar movies based on the plot summaries using NLP and cosine similarity.

🚀 What It Does
You type in a movie name. It looks at the movie's overview, compares it to others, and recommends similar titles.

🔧 How It Works
Dataset: Comes from TMDB, includes title, overview, genre, etc.

Cleaning: Filters out missing data and irrelevant columns.

Text Vectorization: Uses CountVectorizer to convert overviews into vectors.

Similarity: Uses cosine similarity to find and rank similar movies.

Recommendation: Returns top N closest matches to the input movie.

🧰 Tech Stack
Python 3

Pandas

NumPy

Scikit-learn

Jupyter Notebook

📂 Files
movie_recommended_system.ipynb — Main notebook with the full implementation

tmdb_5000_movies.csv — Dataset (make sure it's in the same directory)

README.md — This file

✅ How to Run It
Clone this repo or download the notebook

Install the required packages:

bash
Copy
Edit
pip install pandas scikit-learn
Open movie_recommended_system.ipynb in Jupyter or any compatible editor

Replace the movie name in the last cell with one of your choice:

python
Copy
Edit
recommend('Avatar')
Run the cell to get recommendations.

🧠 Example Output
python
Copy
Edit
recommend('Avatar')
markdown
Copy
Edit
1. Aliens vs Predator: Requiem  
2. Battle: Los Angeles  
3. John Carter  
4. The Helix... Loaded  
5. Star Trek Into Darkness  
📌 Limitations
Only works for movies in the dataset

No personalization — it doesn’t learn user preferences

Relies on overview text only, not cast, ratings, or user data

📈 Future Improvements
Add collaborative filtering

Build a web interface using Streamlit or Flask

Use TF-IDF or advanced NLP techniques (e.g. BERT) for better vectorization

🙌 Credits
Dataset: TMDB via Kaggle
