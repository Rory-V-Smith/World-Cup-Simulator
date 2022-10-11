# World-Cup-Simulator
Simulates the winner of the FIFA World Cup using FIFA Men's World Rankings, per the below.

```
$ python tournament.py 2018m.csv
Belgium: 20.9% chance of winning
Brazil: 20.3% chance of winning
Portugal: 14.5% chance of winning
Spain: 13.6% chance of winning
Switzerland: 10.5% chance of winning
Argentina: 6.5% chance of winning
England: 3.7% chance of winning
France: 3.3% chance of winning
Denmark: 2.2% chance of winning
Croatia: 2.0% chance of winning
Colombia: 1.8% chance of winning
Sweden: 0.5% chance of winning
Uruguay: 0.1% chance of winning
Mexico: 0.1% chance of winning
```

### Background
In soccer’s World Cup, the knockout round consists of 16 teams. In each round, each team plays another team and the losing teams are eliminated. When only two teams remain, the winner of the final match is the champion.

In soccer, teams are given [FIFA Ratings](https://en.wikipedia.org/wiki/FIFA_Men%27s_World_Ranking#Current_calculation_method), which are numerical values representing each team’s relative skill level. Higher FIFA ratings indicate better previous game results, and given two teams’ FIFA ratings, it’s possible to estimate the probability that either team wins a game based on their current ratings. The FIFA Ratings from just before the two previous World Cups are available as the [May 2018 Men’s FIFA Ratings](https://www.fifa.com/fifa-world-ranking/men?dateId=id13792) and [March 2019 Women’s FIFA Ratings](https://www.fifa.com/fifa-world-ranking/women?dateId=ranking_20220805).

Using this information, this programme simulates the entire tournament by repeatedly simulating rounds until we’re left with just one team. And if we want to estimate how likely it is that any given team wins the tournament, we might simulate the tournament many times (e.g. 1000 simulations) and count how many times each team wins a simulated tournament.

Completed in part of Harvard's [CS50 - Introduction to Computer Science, 2020](https://cs50.harvard.edu/x/2020/).
This was Lab 6: [World Cup](https://cs50.harvard.edu/college/2020/fall/labs/6/).
