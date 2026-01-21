# Book-Match: Content-Based Recommendation Engine

This project is a book recommendation system that analyzes metadata from a collection of over 11,000 books. It uses natural language processing techniques to suggest titles based on author similarity and writing styles.

## Features
* Recommendation Engine: Uses TF-IDF vectorization and cosine similarity to find similar books based on author metadata.
* Data Cleaning: Processes raw book data, handles missing values, and filters for quality based on rating counts.
* Interactive Interface: Includes a search function and adjustable results slider using Jupyter widgets.
* System Validation: Contains health checks and accuracy metrics to verify recommendation performance.
* Visual Analysis: Provides data visualizations for rating distributions and author frequency.

## Technical Stack
* Python: Primary programming language.
* Pandas: Used for data manipulation and cleaning.
* Scikit-Learn: Used for machine learning, specifically TF-IDF and similarity calculations.
* Matplotlib: Used for generating data visualizations.
* IPywidgets: Used for the interactive user interface.

## Data Source
The project utilizes a Goodreads dataset containing 11,123 entries. For the recommendation engine, the data is filtered to focus on 8,402 books that have at least 100 ratings to ensure data reliability.

## Implementation Details
1. Preprocessing: Author names are cleaned and formatted into unique tokens for analysis.
2. Vectorization: The system uses TfidfVectorizer to convert text data into a numerical matrix.
3. Similarity Calculation: A cosine similarity matrix measures the distance between different book entries.
4. Search Logic: A sanitized search function matches user input against the filtered dataset to retrieve the most relevant matches.

## Usage
1. Clone the repository to your local machine.
2. Ensure you have the necessary libraries installed: pandas, scikit-learn, matplotlib, and ipywidgets.
3. Open the C964_Capstone.ipynb file in a Jupyter environment.
4. Place the books.csv file in the same directory as the notebook.
5. Run the cells to interact with the search interface.

## Project Results
Testing against known authors (Stephen King, Bill Bryson, and J.K. Rowling) showed high accuracy in retrieving relevant titles within the same series or author ecosystem, with a 100% partial or exact author match rate during validation tests.
