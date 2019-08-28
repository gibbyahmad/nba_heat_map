We all know that the Toronto Raptors are NBA Champions. Toronto has seen great players come through, like Kawhi Leonard, Vince Carter, and many others. But when it comes to producing great players, Toronto lags behind many other major areas. Seeing as there is often a discrepancy between players that play in a city, and that cities ability to produce elite talent, we focused our analysis on creating two different sets of maps - first to visualize the statistics of players that play in a certain area, and also the statistics of players that are born in a certain area.

Questions:

This project will broadly determine which cities have the best teams and produce the best players. It will show the effects of team styles on player statistics, such as more shots being attempted by players on certain teams. It will also show which areas have historically produced the best players based on these characteristics. Insights can be drawn on these to determine why this might be, such as better coaching in certain areas, more basketball programs, more focus on 3 point shooting, etc.

This project will produce 8 heat maps that will show the following information based on teams and players from cities in the continental United States.

Metrics Used: 
3 point %
Field goals %
Rebounds per game
Overall points 

Data:

We knew we would need data on player stats, as well as where the player was from, and the team they played for. Using an external csv with player stats from 1980 to present day, we were able to see the stats of ~2200 players, which we deemed to be a large enough sample to be representative of the cities and teams. 

APIs used:

https://pypi.org/project/nba-api/
From API:
Player name, Team, City of Team, Birth city, various stats
https://developers.google.com/maps/documentation/
From API:
Google maps creator for heatmaps

Additionally, we used the Google Maps API to create the heatmaps.

Data Cleanup & Exploration: 
From here, we obtained an API that had the city of birth of the players, the city of the team that they played for. We then merged the datasets together to give a comprehensive list of the players birthplace, team, and stats, which we could use for analysis.

Problems:
We noticed that the API contained data on some players that played for NCAA teams, and we theorized that the API used the data of the players for the college they played for, if the player was drafted by an NBA team, signed a contract, but never got into a professional game.

We also had to account for team cities of teams that previously were in the NBA but moved to different cities, to be sure not to remove them from the dataset.

Early Findings:
We noticed that a few major areas, like Washington and Philidelphia, accounted for a large proportion of the NBA population that we used for our analysis, which was a good indicator that we were on track to find some trends about where players are from based on the data.

We also noticed that some cities were spelled with acronyms such as LA for certain players, and had to manually manipulate the data to change them so they could be properly grouped.

FInally, we noticed that the sample size of certain areas fluctuated greatly and in proper data viz form we should find a way to account for this on the viz. We decided to change the size of the markers on the map based on the count of players from that area/played in that area, depending on the scope of the map.

Analysis:

Field Goal % by CIty:

Points Per Game by Playing City:

As we can see, the more successful franchises (Miami, Los Angeles, Cleveland) appear with more points.
Total rebounds by Playing City:

As we can see, the longer tenured franchises appear to have more total rebounds, as they had more opportunities to accrue them over more years. Short-lived cities like Vancouver appear to have less rebounds to their name.
3 point percentage by playing city:

Some teams like Miami, OKC and Houston have preached 3 point effectiveness, so it makes sense to see them on the higher side of this list. It appears that GSW even with the two best shooters ever have had many players with poor 3 point shooting percentages which bring them to the lower side of the list.

Player Count by Birth City:

East Coast is much better at producing players. Toronto and Canada lag behind in player development.

Number of Games Played by Top 30 Birth Cities:

Chicago has helped the NBA produce the most games played by players. Toronto does not appear in the Top 30.

Conclusion:

While the Raptors have enjoyed championship level success as a playing city, they are significantly lagging behind in their production of elite-level basketball players.

If Toronto wants a superstar to give them a hometown return one day, they must amp up their levels of grassroot basketball programs and attract elite basketball coaches and development professionals to the city.
