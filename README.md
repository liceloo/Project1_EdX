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

>* H0: There is no difference in mean prize earnings between China and the rest of the world.
>* HA: There is a significant difference in mean prize earnings between China and the rest of the world.
* Results:
* China p-value: 0.5589551168537024 
* Korea p-value 0.00018350593935363384
4. Conclusion
* Since the p-value is less than 0.05, there is sufficient evidence to reject the null hypothesis and conclude that the difference in mean prize earnings by game is significant.
* Since China's p-value is greater than 0.05, we cannot reject the null hypothesis and conclude there isn'y enough evidence to accept that China's mean earnings is different from the rest of the world. This m
* However, Korea's p-value is less than 0.05, so we can reject the null hypothesis and conclude that Korea's mean prize earnings is statistically significant from the rest of the world.

### References
Datasets for earnings: https://www.kaggle.com/code/prbm30/esports-earnings-data-analysis/input?select=highest_earning_players.csv


## Questions 2: If one were to pursue competetive gaming as a career what game should they play? What is the best way to generate income? (Bryan Miller)
This section evaluates twitch information from 2016 to 2023. And looks at highest pools paid per game in tournaments at the end of 2022.

Jupyter Notebook: Bryan E Sport.ipnyb

### References:
            https://www.kaggle.com/code/rankirsh/visualising-twitch/input?select=Twitch_game_data.csv
            https://www.kaggle.com/code/prbm30/esports-earnings-data-analysis/input

step1: Graph Twitch data 2016 - 2023 hours watched and streams available.    Time series popularity of twitch streaming

step2: Graph usd Hours watched vs top 10 Games in period of 2019 - 2023.      Time series popularity of twitch streaming

step3: Merge Data into single graph. Remove NA's and get best games to play if starting E-Sports Career. 


Twitch and total Video Game information not available for Rainbow 6 (newest Game)

## Question 3: (Justin Byrd)


## Question 4: Is E-Sports taking over traditional sports in the US? (Brandon Loredo)
Jupyter Notebook: Project 1.ipynb (Branch - Brandon)

This section compares the earnings betweeon eSports and Active sports earners from the years 2013 to 2021.

1. Processing Data and Cleaning
* All datasets were found on kaggle/esportsearnings (link under references). 

2. Data Visualizations
* Graphed top 10 earners for both esports and active sports for the years 2013-2021 
* Graphed the average top 10 earners for both esports and active sports for the years 2013-2021
* Graphed multiple boxplots/scatter plots to show the distribution of earnings by years

3. Analysis
* Both have a positive slope, which suggest an increase in earnings over time and potential future growth.

* T-test between top 10 earners for both E-sports and Active sports: 
** T-Statistic: -17.67153631041991
** P-Value: 5.132170911238922e-41

4. Conclusion
* Based on the t-statistic and the very small p-value, we can infer that there is a statistically significant difference in earnings between the top 10 esports earners and the top 10 active sports earners. 
* The negative t-statistic suggests that the average earnings of the top 10 esports earners are lower than the average earnings of the top 10 active sports earners. 
* The extremely small p-value indicates strong evidence against the null hypothesis of equal average earnings between the two groups.

### References
Datasets for Esports: https://www.esportsearnings.com/history/2021/top_players

Datasets for Active Sports: https://www.kaggle.com/datasets/darinhawley/forbes-high-paid-athletes-19902021?resource=download
