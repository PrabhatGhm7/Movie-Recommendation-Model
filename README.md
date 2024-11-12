# 🎬 Movie Recommendation System

This repository contains a **Movie Recommendation System** built with Python, leveraging machine learning techniques to suggest movies based on user preferences. The model employs **cosine similarity** on a matrix of movie ratings, enabling recommendations for similar movies based on a selected title.

## 📂 Project Overview

The system uses the [MovieLens 20M Dataset](https://www.kaggle.com/grouplens/movielens-20m-dataset) for training, which includes millions of movie ratings. Our approach focuses on generating high-quality recommendations by creating a movie-user matrix and applying a collaborative filtering technique.

## ✨ Key Features

- **Cosine Similarity Calculation**: Computes similarity scores between movies based on user ratings.
- **Genre One-Hot Encoding**: Extracts and utilizes genre data for better filtering.
- **Easy-to-Use Function**: Just input a movie name, and get the top recommendations instantly.
- **Data Preprocessing**: Handles missing values, duplicates, and applies filtering to retain only movies with a significant number of ratings.

## 🔧 Installation & Setup

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/movierecommendation.git
    cd movierecommendation
    ```

2. **Install Dependencies**:  
    Make sure you have Python installed, then install the required packages.

    ```bash
    pip install -r requirements.txt
    ```

3. **Download Dataset**:  
    The dataset is automatically downloaded via Kaggle API when running the script. Ensure you have Kaggle API configured.

## 🛠️ Usage

- **Load and Run**: After installation, you can run the script directly to test the recommendation function.

    ```python
    # Import the main function
    from movie_recommendation import get_recommendations_by_name

    # Get recommendations
    recommendations = get_recommendations_by_name("Thor", similarity_matrix, movie_rating, top_n=5)
    print(recommendations)
    ```

## 📊 Methodology

- **Data Preprocessing**: Cleans the dataset, handling missing values and duplicates.
- **Matrix Generation**: Creates a sparse matrix using `csr_matrix` to optimize memory.
- **Similarity Calculation**: Applies cosine similarity to find the closest matches for each movie in the dataset.

## 👤 Author

- **Prabhat Ghimire** - [LinkedIn](https://www.linkedin.com/in/yourprofile) | [GitHub](https://github.com/yourusername)

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💡 Contributing

Feel free to submit issues, fork the repository, and make a pull request with your ideas for improvement.
