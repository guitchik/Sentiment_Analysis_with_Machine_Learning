# Studying Sentiment Analysis and its effects on Machine Learning Predictions



##### Group Members: Ram Gollakota, Celeste Terell, Taylor Little, and Timothy Prost



## Motivation and Summary

We used traditional algorithmic trading algorithms, specifically Bollinger Bands, to analyze Apple's stock price (AAPL) and identify potential trading opportunities based on stock price volatility.  We used Random Forest Algorithm to produce a  classification report.

Next, we incorporated sentiment analysis using upvote scores from the subreddit "Wall Street Bets." We ran the Bollinger Bands analysis to identify the entry and exit points.  We also performed the Random Forest predictive model and its classification report.  We compared both approaches to see what difference we could find by incorporating sentiment analysis data.



## Sourcing Data

Wall Street Bets (WSB):  https://www.reddit.com/r/wallstreetbets/

Alpaca Trading:  https://alpaca.markets/



## Collection, exploration, and cleaning process:   
- Web scraping on WSB to get upvote ratios and score data
- Merge the Alpaca daily trading data with the sentiment scores from WSB
- Overcame issues of merging two different time and date-indexed data frames
- Had to address missing data in the sentiment analysis




## Approach

#### Libraries and APIs:  
Pandas, Numpy, Finta, Alpaca Trade API, Requests, PMAW, Panel

#### Breakdown of tasks and roles:  
Ram - Trading and machine learning
Tim - Visualizations
Taylor - Web scraping
Celeste - Git support, Presentation

#### Challenges:
Scraping the WSB subreddit for ticker symbols, dates, times, and up/down votes

#### Successes:  
For Taylor, figuring out how to scrape a website for data, working with indices, and getting time stamping across platforms to work!



## Findings:

- Stock prediction performance decreased slightly by adding sentiment analysis.  The precision-recall scores were 4-5% lower. 

- The number of entry points was 3x more with the sentiment analysis than without. 

#### Overall, our conclusions:
Incorporating sentiment analysis from sites such as WSB in a trading algorithm is possible.  However, the resulting model may be biased toward more "buy" signals than trading "exits."
