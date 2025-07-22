# Runescape-Exploratory-Analysis
# About
This is an exploratory project with a dataset from a video game I used to play. It specifically explores the in-game market(known as the Grand-Exchange).

# Necessary Terminolgy
1.  RS(Runescape) = This is the name of the game. Its an online multiplayer game with an active in-game market where players buy and sell numerous items

2.  OSRS(Old-School Runescape) = This is a different version of the same game, that runs separately from the main game and also has its own in game market. Because more players tend to favor this version, it tends to have a much more active and volatile market than RS.

3.  Grand-Exchange(GE) = This is the in-game market which players buy and sell numerous different items at different prices.

4.  LowAlch(Low-level Alchemy) = A spell in the game that allows the player to liquidate an item on the spot, i.e turn it into a money value equivalent to 40% of the items value in the game(with some exceptions).

5.  HighAlch(High-Level Alchemy) = A spell in the game that allows the player to liquidate an item on the spot, i.e turn it into a money value equivalent to 60% of the items value in the game(with some exceptions).

6.  ROI(Return on Investment).

7.  Free Player = There are two types of players in the game, one of them is the free player, they are restricted in terms of certain items they can own or purchase.

8.  Member = This is the second type of player that pays a subscription to be a member, they have access to all aspects of the game and its items. Some items are specifically member only and can therefore only be purchased and wielded by them.
# Process/Initial Steps
Now when I first began this project my first thought was how do I even get this data, surely there must be some way to acquire game data that is reliable and gives up to date information.

1. Researched ways of spooling/acquiring RS/OSRS data.(Web Scrappers or API).

2. Discovering that most of RS3 and OSRS data can be found in json dump that gets regularly updated by runescape itself allowing for easy refresh of data

3. Performed connection by web, using link to the json files

4. Began transformations on the data

# Transformations
Initially when pulling in the json data, it came as a list that had to be converted in to a table, and records that had to be expanded out 
<img width="853" height="706" alt="image" src="https://github.com/user-attachments/assets/a7ae72ea-c7c9-41ff-b848-155845f205cf" />
<img width="1303" height="711" alt="image" src="https://github.com/user-attachments/assets/2f9251ea-c20c-4843-b85f-ae99f222245c" />
Some column data types containing numeric values for calculations also needed to be cleaned so they could be used later.
# Aspects Explored
When making this report, I wanted to make something that would be relevant to the person playing the game and utilizing the games market. One of the major things for a player, be they be a free player or a member is making in game money and the most efficient methods of doing so, when doing this they have to consider things like the value of the item and the price of the item on the Grand Exchange. Note that these are two different things. Items can be obtained through other means besides just the Grandexchange, meaning they can be purchased from NPCs. Fortunately my data source includes this price in its output. Now the player would want to know the most effecient way to obtain an item, how much they could buy it for on the market, how much they would get when they LowAlch or HighAlch it and what the return on the investment is of getting the 'raw materials' involved in the process in the first place.
