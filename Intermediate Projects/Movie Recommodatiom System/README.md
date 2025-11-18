🎬 Movie Recommendation System

A simple, effective Python-based movie recommendation engine that suggests similar movies using genre-based cosine similarity. 
It is beginner-friendly, lightweight, and runs completely on the console without requiring external libraries.

📌 Overview
This system recommends movies similar to a user-selected movie using genre vectors and cosine similarity. Each movie is represented by a genre vector (1 if genre exists, 0 if not), and similarity is calculated mathematically.
The project includes 50+ movies, covering:
✔ Sci-Fi
✔ Action
✔ Adventure
✔ Drama
✔ Comedy
✔ Animation
✔ Fantasy
✔ Thriller
✔ Romance

🚀 Features
✅ Add movies with title, genres, and description
✅ Builds a unique set of genres automatically
✅ Converts genres into numerical vectors
✅ Computes cosine similarity between movies
✅ Recommends top 5 similar movies
✅ Fully CLI-based — no external UI required
🧠 How the Recommendation Works
1. Create Genre Vector

If the total genre set is:
[action, drama, sci-fi, comedy]
And the movie genres are:
["action", "sci-fi"]
Then vector =
[1, 0, 1, 0]

2. Sort Results & Show Best Recommendations

Top N movies (default 5) are displayed with their similarity scores.

🏗 Project Structure
movie_recommender/
│
├── Movie Recommodatiom System.ipynb           
└── README.md                                 

🧩 Technologies Used
Python
OOP (Classes & Objects)
Math (cosine similarity)
Genre vectorization

📦 How to Run
1. Save the code as:
movie_recommender.py

2. Run the script
python movie_recommender.py

3. Enter any movie from the list
Example:
Inception
Interstellar
The Matrix
The Lion King
Avengers: Endgame

📁 Dataset Details

Over 50 movies with:
Title
Genres
Description
Genres include:
Sci-Fi, Action, Drama, Crime, Thriller, Comedy, Animation, Adventure,
Fantasy, Romance

🔧 Customization
You can modify:
What	How
Add new movies	Add entries in sample_movies
Number of recommendations	Change top_n in recommend()
Similarity logic	Replace cosine similarity with Jaccard, Euclidean, etc.
Use descriptions too	Add NLP vectorization later
⚠ Limitations
Only genre-based (does not use description text)
Cosine similarity used only for genres
Exact movie name must be typed
Not a machine learning model

🚀 Future Enhancements
You can upgrade this project with:
🔹 NLP-based description similarity
Using TF-IDF or BERT sentence embeddings.
🔹 Hybrid Recommender
Genres + Description + Popularity.
🔹 GUI (Tkinter / Web App)
Turn it into a full application.
🔹 Search-as-you-type
Improve input flexibility.

🏁 Conclusion
This project is an excellent introduction to:
✔ Recommender systems
✔ Cosine similarity
✔ Vector encoding
✔ Object-Oriented Programming
It’s fast, simple, and perfect for portfolio demonstration.
