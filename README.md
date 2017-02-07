# Applied Data Analysis Project: The evolution of a League of Legends player

## Context

League of Legend (LoL) is a multiplayer online is a multiplayer online battle arena video game developed and published by Riot Games for Microsoft Windows and OS X. In League of Legends, players assume the role of an unseen "summoner" that controls a "champion" with unique abilities and battle against a team of other players or computer-controlled champions. The goal is usually to destroy the opposing team's "nexus", a structure which lies at the heart of a base protected by defensive structures. Each League of Legends match is discrete, with all champions starting off fairly weak but increasing in strength by accumulating items and experience over the course of the game. 

The complexity of a LoL match can grow as the players involve get more knowledge of the game and improves their "skill" with a champion. This is why the game is divided in "leagues" or "tiers with 5 divisions in each (V-I): Bronze, Silver, Gold, Platinum and Diamond. Above Diamond there are the "professional tiers" (Master and Challenger) in which people roughtly dedicate more than 8 hours per day playing the game, with the Challenger tier hosting only 200 players for each region.

The cultural relevance in the western and oriental culture is remarkable as in September 2016 the company estimated that there were 100 million monthly active players worldwide. With an player database of the 11,94% of the korean population or the 5,88% of the China's. League of Legends has an active and widespread competitive scene as a "e-sport". In North America and Europe, Riot Games organizes the League Championship Series, located in Los Angeles and Berlin respectively, which consists of 10 professional teams in each continent. Similar regional competitions exist in China, South Korea, Taiwan, South America, and Southeast Asia. The 2016 World Championship's total prizepool was over 5 million dollars, with over 2 million going over to the winner of the tournament. 

## Abstract
 
This project will use data provided by Riots Games https://developer.riotgames.com/ about League of Legends players match history, only in the EUW (Western Europe) server. The objectives are to develop an understanding of LoL player skill evolution over time in terms of their ability to use advanced game features (e.g., runes, masteries, etc.) as well as an understanding of the causes for dropping or continuing to play the game in the long term.

The number of variables in a League of Legends match is huge and can be cuantitative (champions picked and lanes matchups, item build, number of vision wards placed, gold earner per players by kills, assists or objectives...) or qualitative (team communication, teamwork, luck, connection health,...). We will only take into account the most relevant quatitative stadistics. 

In the first phase of the project we will get the data using the Riot API and peform all the Data Wrangling process necesary to then analyze the data. The Data retrieved will correspond to the current (2015-2016) and past season (2014-2015) of competitive matches. In the second phase we will analyze the data to choose the most suitable stadistics to determine a player permormance. Then, for this stadistics, we will choose the Machine Learning aproach that fits the data and try to predict
the results. In the last phase, we will try to visualize the data and drive some conclusions. 

## Data description
Our starting point will be the IDs of a summoner of each Tier (Bronze, Silver, Gold, Platinum, Master and Challenger). For each one, we'll retrieve the League they're located in and we'll retrieve the IDs of every other summoner in those leagues. Once this is done, we'll have a pool of LoL players, balanced between all the possible Tiers. 

For each Summoner we'll get his Name, Tier and Division as basic information and then his Stats and Matchlist, organized by Season. Thanks to the Stats we'll be able to determine the average and aggregate statistics of the player for every Champion he has ever played ever. With the Matchlist, we'll be able to iterate through all the matches played by the Summoner during a certaing Season to get information regarding his position, runes, masteries and team (friendly and opposite) information.

All this data will be properly organized to be queried and used depending on what we need to get and analyze in different stages of the project.

## Feasibility and Risks

Given the huge amount of data available and all the variables that decide the outcome of a match, It could be difficult to select the features that infuence the most the predicition. A not accurate or wrong prediction is possible. 

Limitating the scope of the project can result in an insufient amount of different players data but taking a lot of players can result in a Big Data problem. 

## Deliverables
During the project, 3 IPython notebooks will be done. Those notebooks are:
* Data Mining notebook: Where the data of the LoL's Api will be extracted and saved using DataFrames, Requests and others libraries. Besides, the data will be cleaned to chose the most revelant or the necessary attributes for future use.

* Data Analysis notebook: Where the collected data will be analyzed to select some features, which will be used to make the Machine Learning notebook.

* Machine Learning notebook: will be done taking into account the datasets dimensions. A list of pros and cons for each classifier will be done in order to make an assesment of which classifier fits better our data model. 

* Result Visualization notebook: From the data extracted in the previous notebook, it will be displayed using graphs and, if possible, interactive graphics.
