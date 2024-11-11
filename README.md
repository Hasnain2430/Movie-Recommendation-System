# IMDb Movie Recommendation System

This project is a web scraping tool and recommendation system designed to help users find movies based on their preferences. The program scrapes data from IMDb's "Most Popular Movies" page, gathering details about each movie and storing them in a Pandas DataFrame. Users can specify their preferences, and the system will filter the movies accordingly to recommend the best match.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Data Fields](#data-fields)
- [Example Output](#example-output)
- [Disclaimer](#disclaimer)
- [Contributing](#contributing)
- [License](#license)

## Features

- Scrapes IMDb's "Most Popular Movies" page to gather movie data.
- Collects details including movie title, runtime, rating, age restriction, genre, writer(s), director(s), and trivia.
- Stores the data in a Pandas DataFrame for further analysis and filtering.
- Prompts the user for movie preferences (e.g., genre, minimum rating, maximum runtime, age restriction).
- Filters the DataFrame based on user preferences and recommends a movie.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Hasnain2430/IMDb-Movie-Recommendation-System.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download and set up [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads) (or use WebDriver Manager for automated setup).

## Usage

1. Open the main script (`movie_recommender.py`) in a Jupyter Notebook or similar environment.
2. Run each cell in sequence to start scraping movie details and build the recommendation system.
3. After scraping, you’ll be prompted to enter your movie preferences:
   - **Genre**: Specify your preferred genre (e.g., Action, Comedy).
   - **Minimum Rating**: Set a minimum IMDb rating for your recommendations.
   - **Maximum Runtime**: Define the maximum runtime in minutes.
   - **Age Restriction**: Enter an age restriction preference (e.g., '15', '12A', 'PG', '18', 'R', 'U').

4. The program will filter the movies according to your preferences and recommend a movie that best matches your criteria. If no match is found, a random movie from the original DataFrame will be recommended.

## Data Fields

The tool collects the following data fields:

- **Movie Titles**: Title of the movie.
- **Runtime**: Duration of the movie.
- **Rating**: IMDb rating.
- **Age Restriction**: Age restriction for the movie.
- **Genre**: Genre of the movie.
- **Writer(s)**: Writers of the movie.
- **Director(s)**: Directors of the movie.
- **Fun Movie Trivia**: Trivia about the movie (if available).

## Example Output

The output is displayed in a DataFrame format, filtered according to the user's preferences. For instance, if a user specifies a preference for action movies with a rating above 7.0, a runtime under 120 minutes, and an age restriction of '15', the program will display matching recommendations.

## Disclaimer

The scraper may not work properly or may require adjustments if the HTML structure of the IMDb website has changed. Please inspect the page structure and update the XPath or CSS selectors as necessary.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request to improve the project.
