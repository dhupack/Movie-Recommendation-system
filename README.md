# Movie Recommender System

A machine learning project that recommends movies based on user preferences using the TMDB 5000 dataset. Built with Python and Jupyter Notebook.

## Features
- Content-based movie recommendations
- Uses TMDB 5000 Movies and Credits datasets
- Interactive analysis and visualization in Jupyter Notebook
- Easy to extend for collaborative filtering or hybrid approaches
- REST API for movie recommendations

## Dataset
- [tmdb_5000_movies.csv](tmdb_5000_movies.csv): Contains movie metadata (genres, keywords, overview, etc.)
- [tmdb_5000_credits.csv](tmdb_5000_credits.csv): Contains cast and crew information

## Installation
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd movie-Recommender
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
### Jupyter Notebook
1. Open `movie-recommender.ipynb` in Jupyter Notebook or VS Code.
2. Run the notebook cells to:
    - Load and preprocess the data
    - Build the recommender model
    - Get movie recommendations

### API
The project includes a REST API for programmatic access to movie recommendations.

#### Example Endpoints
- `POST /recommend` — Get movie recommendations by providing a movie title.

#### Example Usage
Send a POST request to `/recommend` with JSON:
```json
{
   "title": "Avatar"
}
```
Response:
```json
{
   "recommended_movies": ["Titanic", "Star Wars", "Interstellar", ...]
}
```

#### Running the API
1. Start the API server (see notebook or script for details).
2. Use tools like Postman or `curl` to interact with the API.

## Example
- Input: Movie title (e.g., "Avatar")
- Output: List of similar movies recommended

## Project Structure
```
movie-recommender.ipynb   # Main notebook
requirements.txt          # Python dependencies
TMDB_5000_movies.csv      # Movie metadata
TMDB_5000_credits.csv     # Cast and crew data
```

## Requirements
- Python 3.7+
- Jupyter Notebook
- pandas, numpy, scikit-learn, etc. (see requirements.txt)

## Credits
- [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-dataset)

## License
This project is for educational purposes. Please check dataset license for usage restrictions.
