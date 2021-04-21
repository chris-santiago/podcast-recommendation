# GuidePod

Description of the project

## Installation

To install this package, use the following:

`$ python -m pip install git+https://github.com/gzhhu/podcast-recommendation.git`

Then navigate to the project directory and install the dependencies: 

`$ python pip install -r requirements.txt `

## Scraping, data processing, and modeling

Script | Description | Output
:----- | :---- | :------
1 - Scraping/get_podcast_names.ipynb   | Scrape the top 200 podcast IDs of each genre. | `podcast_ID_list.csv`
1 - Scraping/get_podcast_reviews.ipynb   | Scrape the first 500 reviews for each podcast in `podcast_ID_list.csv`. | `GuidePod.sqlite`
1 - Scraping/get_podcast_feedinfo.ipynb   | Scrape feed information for each podcast in `podcast_ID_list.csv`. | `GuidePod.sqlite`
1 - Scraping/get_podcast_episodes.ipynb   | Scrape episode data for each podcast in `podcast_ID_list.csv`. | `GuidePod.sqlite`
2 - Cleaning/cleaning.ipynb   | Clean `GuidePod.sqlite` and join tables. | `GuidePod_clean.sqlite`
3 - Modeling + Data Prep/preprocessing.ipynb   | Feature engineering and selection. | `podcast.csv`
3 - Modeling + Data Prep/recommendations.ipynb   | Build the recommendation model. | `recommendations_top10.json`
3 - Modeling + Data Prep/word counts.ipynb   | Identify the most frequently used words. | `top100_words.json`

## Running the web application

...
