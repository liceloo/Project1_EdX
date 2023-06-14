# Project1 - this project explores the data associated with E-Sports.

## Introduction:
Let's say your friend is fed up with his 9-5, and wants to become a professional gamer. Let's dive into see what his best odds are for his future career.

## Question 1: Which game has the most overall earnings? (Alice Liu)
This section dives into how tournament prize earnings is statistically distributed. Tournament prize money is a source of revenue for most professional players.  For example, Fortnite World Cup 2019 had a total prize pool of $30 million.

1. Processing Data and Cleaning
* All datasets were found on kaggle (link under references) and nans were dropped. 

2. Data Visualizations
* Graphed games by overall tounrnament prize money 
* Graphed the top 15 players by overall tournament prize money and color coded by game
* Graphed multiple boxplots to show the distribution of tournament earnings by game
* Geographically plotted the countries, colored by total overall prize earnings. 

3. Analysis
* The first two visually showed that Dota 2 seemed to dominate this earnings category, so I ran an ANOVA test to see if it was true.
* H0: There is no difference in mean prize earnings between each game.
* HA: There is a significant difference in mean prize earnings between each game.
F_onewayResult(statistic=133.62075399715448, pvalue=7.125113359124046e-16)

* The geographical plot visually showed that China and Korea earn much more than the rest of the world. I ran two different Z-tests to confirm whether this was true.
>* H0: There is no difference in mean prize earnings between China and the rest of the world.
>* HA: There is a significant difference in mean prize earnings between China and the rest of the world.
**--------------------------------------------------------------------------------------------------------**
>* H0: There is no difference in mean prize earnings between China and the rest of the world.
>* HA: There is a significant difference in mean prize earnings between China and the rest of the world.
* Results:
* China p-value: 0.5589551168537024 
* Korea p-value 0.00018350593935363384
4. Conclusion
* Since the p-value is less than 0.05, there is sufficient evidence to reject the null hypothesis and conclude that the difference in mean prize earnings by game is significant.
* Since China's p-value is greater than 0.05, we cannot reject the null hypothesis and conclude there isn'y enough evidence to accept that China's mean earnings is different from the rest of the world. This m
* However, Korea's p-value is less than 0.05, so we can reject the null hypothesis and conclude that Korea's mean prize earnings is statistically significant from the rest of the world.


Questions 1) If one were to pursue competetive gaming as a career what game should they play? What is the best way to generate income?
          2) Will E-Sports eventually overtake conventional sports?
          



Twitch and total Video Game information not available for Rainbow 6 (newest Game)

### References
Datasets for earnings: https://www.kaggle.com/code/prbm30/esports-earnings-data-analysis/input?select=highest_earning_players.csv
