# 🎬 Movie Recommendation System  

This is a **Movie Recommendation System** built using **Streamlit, Pandas, and TMDb API**. It suggests movies based on similarity scores calculated using a precomputed similarity matrix.  

## ✨ Features  
- Select a movie from the dropdown, and the system recommends 5 similar movies.  
- Fetches movie posters dynamically using the TMDb API.  
- Utilizes a **pretrained similarity model** stored in `similarity.pkl` for recommendations.  
- Interactive UI powered by **Streamlit** for an engaging user experience.  

## 🛠 Tech Stack  
- **Python** (pandas, requests, pickle)  
- **Streamlit** (for the web interface)  
- **TMDb API** (for fetching movie posters)  

## 📂 Understanding the `.pkl` Files  
This project uses two **pickle (`.pkl`) files** to store preprocessed data:  
1. **`movies_dict.pkl`** – Stores a dictionary containing movie details, such as movie titles and their corresponding IDs. This is loaded into a Pandas DataFrame for easy access.  
2. **`similarity.pkl`** – Stores a precomputed similarity matrix, which helps in efficiently finding similar movies based on content-based filtering (e.g., cosine similarity).  

By using these `.pkl` files, the recommendation system avoids recalculating the similarity matrix every time, making the app faster and more efficient.

## 🚀 How to Run  
1. Clone the repository  
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/movie-recommender.git
   cd movie-recommender
   ```  
2. Install dependencies  
   ```bash
   pip install -r requirements.txt
   ```  
3. Run the Streamlit app  
   ```bash
   streamlit run app.py
   ```  

## 📌 Notes  
- Ensure you have `movies_dict.pkl` and `similarity.pkl` in the project directory.  
- Replace the API key in `fetch_poster()` with your own TMDb API key.  

💡 Feel free to contribute, fork, and improve the project! 🚀
