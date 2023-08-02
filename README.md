# TransferMarket

In this project we crawl lots of data from transfermarket.com to build data base for implementing several Statistics and Ml models to analysis the whole data 

### this project includs four main phases : 
#### 1- Crawl and collect the data
#### 2- Design Data Base
#### 3- Statics Analysis
#### 4- Predict and evaluated with ML tools



## Crawl Section
crawl and collect all the data includs: players, teams, matches, .... for five main countries :England , Germany , French ,Spain , Italy.

## Desing Data Base
clean the whole collected data and prepare them to build data base using SqlAlchemy library in python 

## Statistics Analysis 
### 1-Descriptive statistics 
  
    1. Get the distribution of the number of games players play in a season. Also show what percentage of games the players participated in.
    2. Check the relationship between the number of goals scored and the site's estimated price for a player (use linear regression for this).
    3. Obtain the estimated price distribution of the players by disaggregating the players' positions.
    4. Get the number of goals scored in different leagues.

###  2-Expert request 
  
    1.One of the experts wants to know how accurate the transfermarkt site is in estimating the players' prices. Also, recently there has been a problem in the football industry 
      where players are traded for much more than their real value. For this reason, in this section you are     
      asked to compare the distribution of estimated prices of players sold per season, and the actual price of transfers per season (omitting free transfers).

###  3-Players request
  
    1. Let's say that a striker wants to change his team, and for that reason, he searches for teams that need a striker. The need of an attacker is presented in such a way that         the performance of the players in the attack is worse than the performance of the players in the defense. Any team that has this feature is considered a suitable option. 
       Also, teams should be sorted based on their need for strikers. That is, 
       the team that has a greater difference in defense and attack performance should be ranked higher.
        *Pay attention that in this section you have to design a measure for the performance of the players! Your criteria can be different       
       according to the post of the players!

###   4-Coach request 
   
     1. A coach plans to strengthen the team for the next season. For this reason, you are asked to find players who have performed very well and at the same time, have a low 
        price.To do this, you need to find players that are in the top 30% in terms of performance but in the bottom 
        40% in terms of price.
     2. Compare the player price distribution chart you obtained in the first part with the entire player community.
     3. Compare the post distribution of the players you got in the first part with the total player community.
     4. The coaches of the champion teams of the top 5 European leagues have requested to find the players who did not perform well in their teams. To do this, find outliers based on   
        the criteria you designed to measure player performance, and find players who performed worse than other players.


###  5-Hypothesis testing

     1- One of the most frequent phenomena in football is the inappropriate performance of young players after transferring to a new team. There are countless talented footballers who           are transferred to big teams for a huge fee, but their performance does not go as expected at all. For this reason, one of the things that coaches believe is that experienced            players are better suited than young players for a short period of time (for example, a season), because they perform better in a short period of time. Consequently, they have           given you the following hypothesis and asked you to validate their hypothesis.

        Experienced players (at least 30 years old) in their first season with a new team generally perform better than less experienced players (less than 30 years old) in their first          season with a new team.

        Obviously, you have to provide a suitable measure of player performance and then test this hypothesis. After the statistical analysis of the hypothesis, give at least 3                  justifications for the result you got (the same as the justification given in the introduction of this section for the claim of attackers with different heights). Be careful             that your results and your arguments depend on the criteria you define. In this section, you should use data from the seasons 2018-2017 to 2021-22.


      2- One of the objections to the Champions League is that the top teams of each league participate in the competition, and are paid for their participation. As a result, stronger 
         players prefer to go to these teams to gain more attention from the fans, as well as receive more money in salary. As a result, experts claim that the teams in the European              Champions League perform better than other teams. In fact, you are asked to test this hypothesis:

         The performance of the teams in the European Champions League is better than other teams in the league.

         To do this, you must first design a benchmark for team performance and then compare the performance of the teams in the league with other teams in Europe's top 5 leagues. In 
          this section, use the data for the 2021-2022 season.
        
      3- As players get older, they are more at risk of injury and their injuries take longer to heal. Also, older players usually have less physical ability and can play less than               younger players. For this reason, the average age of the teams is a very important factor and coaches always attach great importance to this criterion.

         According to the above arguments, experts believe that coaches who have older teams (have a higher average age), use players in rotation, and as a result, get more players in 
         the game. Using the data provided, test the following hypothesis:

         Players who have participated in at least 20% of the team's games are considered active. If the average age of the team players increases, the number of active players also 
         increases.To test this hypothesis, first you need to group the teams in the top 5 leagues based on the average age of the team (i.e. if we consider the average age of the team 
         as a random variable, you need to divide the teams into several groups by discretization. You can For example, do this based on 2-year intervals. It is up to you to choose this 
         interval). Then, for each team, calculate the number of active members and then check the distribution of the numbers of different categories together. In this section, use 
         data from the 2021-2022 season.


## Machine Learning 
 ### 1- Predict players market value
     1. The goal of this problem is to create a machine learning model that can predict players' market value based on characteristics and recent transfer data. Market value represents 
        the estimated value of a player in the transfer market. By predicting market value, teams, agents and other stakeholders can make informed decisions during player transfers.
 ### 2- Players position classification
     1. In this problem, the goal is to develop a classification model that can accurately classify players into different positions (e.g., forward, midfielder, defender) based on their         characteristics and playing history. Classification of players into positions can help with team formation, player recruitment and tactical decisions in football.
 ### 3- Similarity clustering of players
     1. The purpose of player similarity clustering is to group players based on their characteristics and playing styles to identify similar characteristics among them. This can help           with player scouting, team formation and tactical decision making. By grouping players with similar attributes, teams can identify potential transfer targets or find suitable            replacements for specific situations.
