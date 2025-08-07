# movie_recommender_system

Movie Recommender System
This project is a content-based movie recommender system built using Python. It takes a movie title as input and recommends similar movies based on the overview and other metadata using NLP and cosine similarity.

🚀 What It Does
You enter the name of a movie, and the system gives you a list of similar movies you might enjoy. It does this by analyzing the descriptions (overviews) and computing similarity scores.

🔧 How It Works
Dataset: Pulled from TMDB with metadata like title, overview, genres, etc.

Data Cleaning: Missing values are handled. Only relevant columns are selected.

Text Processing: Movie overviews are transformed into vectors using CountVectorizer.

Similarity: Cosine similarity is used to find and rank similar movies.

Recommendation Logic: Top N similar movies are shown based on a selected movie.

🧰 Tech Stack
Python 3

Pandas

NumPy

Scikit-learn

Jupyter Notebook

📂 Files
movie_recommended_system.ipynb: Main notebook with the complete implementation.

tmdb_5000_movies.csv: Dataset with movie metadata (you'll need this to run it).

README.md: You're reading it.

✅ How To Run
Clone the repo or download the notebook.

Make sure the required libraries are installed:

bash
Copy
Edit
pip install pandas scikit-learn
Run the notebook:
Open movie_recommended_system.ipynb in Jupyter Notebook or any compatible editor.

Replace the movie title in the last cell with your favorite movie and run the cell to get recommendations.

🧠 Example Output
Input:

python
Copy
Edit
recommend('Avatar')
Output:

markdown
Copy
Edit
1. Aliens vs Predator: Requiem
2. Battle: Los Angeles
3. John Carter
4. The Helix... Loaded
5. Star Trek Into Darkness
📌 Limitations
Only works with the movies present in the dataset.

Recommendations are based purely on content (text), not user behavior or ratings.

📈 Future Improvements
Add collaborative filtering.

Integrate with a web interface using Streamlit or Flask.

Improve NLP using TF-IDF or word embeddings.

🙌 Credits
Dataset: TMDB
