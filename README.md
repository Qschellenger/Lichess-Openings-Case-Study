# Lichess-Openings-Case-Study
Case Study for the Google Data Analytics course offered through Coursera.org. 




# Introduction
I chose to analyze popular Chess first moves on Lichess.org for 1,500 elo rated players and below. The public data set from https://www.kaggle.com/datasets/datasnaek/chess was used, it was generated via Lichess's public API. I created the project myself to get a better understanding of R and also chess as I am slowly learning how to play.

# Scenario
You are starting to learn chess after doing puzzles for a few weeks. Upon looking up proper openings and what beginner techinques you should learn, you realize there is so much information surrounding chess, given its long history. In an attempt to get better aquianted with the game, you want to simplify your learning down to one opening move that you can specialize in to give you the best chance of winning games early on.

# Ask
To mitigate the overwhelming initial learning of chess, is there a specific opening move when you are playing as White, that would give you a higher win rate?

# Prepare Phase
Data:
Lichess.org is a free website that allows users to play chess in a variety of different ways. They host games in all different time constraints along with some puzzles and lessons. Lichess also has a public API that was used to gather the data for this project. The Kaggle user "Mitchell J" published a data set of 20,000 games collected from lichess.org to Kaggle.com which was used for this project. This data set can be found: https://www.kaggle.com/datasets/datasnaek/chess . Thank you again for getting compiling this data and allowing others to use it. 
The data is in .csv format and generated from users of the top 100 teams on Lichess.org five years ago.

# Process Phase
R was used for cleaning the data and generating the graphics. R was selected since it is new to me, used in the Coursera Course, and I wanted to get a more in depth understanding of how I could use it not only to clean the data but to generate graphics as well. 

Cleaning:
After verifying that there were no gaps in the data, I started with filtering the data down to what I needed.

Filters and Reasoning:
Only rated games - Since there is both a rated and unrated section on lichess, I wanted to capture only the rated games, since there is an actual elo rating tied to the users and these games would exhibit when users are actively focused on playing the game since their rating is on the line. 

User rating of 1,500 or less for both white & black players - Being new to chess, all new players start at 0 rating and as they play more games and learn more, their rating improves. New users tend to be less than 1000 rated, with that in mind I wanted to allow myself more room to grow in anticipation that I continue to learn the game for years to come. I also didn't wanted to restrict the data by too much and create a sample size that was too small.

Removed games that resulted in Draws: Since draws can commonly occur in chess, and there is no winner in them, I wanted to remove them from the pool all together. This would allow an appropriate win/loss rate to be generated since a draw is not included as either.

# Analyze
The final data analyzed contains over 4,000 games played where all filtered criteria was met. R was also used to generate graphics to help articulate what is the outcome from the different opening moves.



