# Man-Utd-Fan-Satisfaction-Levels-First-19-games

A visualization of how much Manchester United fans enjoyed each game from the first half of the 21/22 Premier League season.

### Process:
Satisfaction ratings were gauged by running a sentiment analysis on replies to Manchester United's main Twitter account (@ManUtd). After every game, Man Utd's Twitter account
posts a tweet with the final scoreline. The replies to those tweets were scraped using the scraper and only those tweets were analyzed for every game.

The code is designed to scrape and analyze replies to one tweet only. So the process was repeated 19 times for each game.

After extracting the replies, I used TextBlob to assign a polarity value to each reply which could be positive or negative. Then I took a sum of all the polaritiesto get a net value of total polarity for the match day. The sum was then adjusted for number of replies as every game does not have the same number of replies. The final value was calculated under the variable name: "Per".

Results for each match day were added to the excel file --> Sentiment Analysis.xlsx
Further analyses were performed to assign a value of satisfaction levels by looking at which percentile they ranked in

Results were visualzed on a bar chart using Excel and PowerPoint



### Files:
1. Sentiment Analysis.ipynb: Python file with the scraper AND the initial calculations to calculate the polarity of fan's reactions to each game
2. Sentiment Analysis.xlsx: Excel file that contains calculations used to assign a satisfaction rating on a scale of 1-5. 
3. Man Utd satisfaction ratings Viz.png: Bar chart showing results
