# Applied Data Analysis Project: The evolution of a League of Legends player

##Abstract
This project will use data provided by Riots Games https://developer.riotgames.com/ about League of Legends players match history. The objectives are to develop an understanding of LoL player skill evolution over time in terms of their ability to use advanced game features (e.g., runes, masteries, etc.) as well as an understanding of the causes for dropping or continuing to play the game in the long term.
##Data description
Our starting point will be the IDs of a summoner of each Tier (Bronze, Silver, Gold, Platinum, Master and Challenger). For each one, we'll retrieve the League they're located in and we'll retrieve the IDs of every other summoner in those leagues. Once this is done, we'll have a pool of LoL players, balanced between all the possible Tiers. 

For each Summoner we'll get his Name, Tier and Division as basic information and then his Stats and Matchlist, organized by Season. Thanks to the Stats we'll be able to determine the average and aggregate statistics of the player for every Champion he has ever played ever. With the Matchlist, we'll be able to iterate through all the matches played by the Summoner during a certaing Season to get information regarding his position, runes, masteries and team (friendly and opposite) information.

All this data will be properly organized to be queried and used depending on what we need to get and analyze in different stages of the project.

##Feasibility and Risks
##Deliverables
##Timeplan

|                           | 31 Oct - 6 Nov | 7 - 13 Nov | 14 - 20 Nov | 21 - 27 Nov | 28 Nov - 4 Dec | 5 - 11 Dec | 12 - 18 Dec | 19 - 25 Dec | 26 Dec - 1 Jan | 2 - 8 Jan | 9 - 15 Jan |
|---------------------------|----------------|------------|-------------|-------------|----------------|------------|-------------|-------------|----------------|-----------|------------|
| Propuse                   |  in progress              |            |             |             |                |            |             |             |                |           |            |
| Data Extraction           |                |in progress            |             |             |                |            |             |             |                |           |            |
| Data Inspection & Roaling |                |            |in progress             |             |                |            |             |             |                |           |            |
| Data Analysis             |                |            |             |  in progress           | in progress               |            |             |             |                |           |            |
| Machine Learnig           |                |            |             |             |                |   in progress         |            in progress |             |    in progress            | in progress          |            |
| Result Visualization      |                |            |             |             |                |            |             |             |                |           |  in progress          |