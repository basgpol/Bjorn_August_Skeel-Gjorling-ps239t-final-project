# ps239t-final-project
Project detecting presence of Game Framing in Danish Parliamentary Debates since 2007

## Short Description

Several studies with the political science literature have shown that framing politics creates political cynicism and distrust among voters. But not studies, to my knowledge have investigated if and how politicians themselves have contributed to the increasing focus on the “game of politics”. This project investigates how the presence of “the game frame” in Danish parliamentary debates have changed over time and if its presence varies according to the political environment (is there an upcoming election?).

The project relies heavily on computational tools. First, I create several functions using Python that enable me to scrape transcripts of parliamentary debates in Denmark since 2007. Second, I create another function in Python that calculated the proportion of “game frame words” used in these debates. Third, I use R to visualize my findings and conduct statistical analysis.

I find that the presence of game framing has a cyclical nature. Danish politicians use game framing more in periods of parliamentary elections. This is supported by a statistically significant negative association between game frame presence and days to nearest election. The closer to an election, the more do Danish politicians use game framing. This indicates that Danish politicians themselves contribute to the “problem of game framing” which increases political cynicism and distrust among voters.

## Dependencies

Software that my code depends on:

1. R, version 3.2.
2. Python, version 3.6, Anaconda distribution.

## Files

List of files in the repo:

#### Data

1. debate_game_frame.csv: Contains data on the date of each debate and the proportion of game frame words
    - *Time*: The date and time of the parliamentary debate
    - *Game frame proportion*: The proportion of game frame words of all non-stop words in the debate.

#### Code

1. 01.scraping.ipynb: Scrape transcripts of Danish parliamentary debates from the official website of the Danish Parliament and save the raw text data as a pickle-object (not possible to upload to github due to large filesize).
2. 02.text_analysis.ipynb: Calculate the proportion of game frame words in each debate. Export the dataset to the file debate_game_frame.csv.
2. 03.visualizations_and_findings.Rmd: Visualize the findings and conducts a statistical test. Results can be found in the Results directory.

#### Results

1. XX 
2. XX 

## More Information

Note: It was not possible to upload the raw text data on all the transcripts scraped in 01.scraping.ipynb to Github due to a very large file size. The data can be reproduced by running the Jupyter Notebook yourselves. This project was created as an exam project for at graduate course at University of California, Berkeley. The course repo is available here: https://github.com/ribernhard/PS239T.

