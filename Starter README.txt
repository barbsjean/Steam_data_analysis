Dates of initial API calls: 5/13/2024 - 5/26/2024

*** i feel like the most important thing you can say about a game is how often it is played. It may have a lot of reviews sure... but how many hours you put into a game speaks volumes about said game. maybe i should focus my main analyis on the avg playtime in the last 2 weeks(maybe lifetime) because THAT to me would be the most important thing about a game.

*** to go along with the above comment... to "own" the game on Steam is important to the analysis and that is what the top_100_2_weeks/forever is ranked by and the top 100 forever is bascially the same as top_100_owned. So steamspy is going off of OWNED games at the measure for best games. I agree to an extent. I feel like the positive reviews AND the mins of playtime are ultimately important. From a business standpoint, the game being bought is most important. However, wouldn't you also want your game to be played as well? Not just owned?

*** notice a change in reviews in Team Fortress... there is a tag going on social media #FixTF2. [save.tf]

*** why is the 2mil - 5 mil owner bucket have the most positive reviews with only 391 games?
			 get a percentage postitive + negative and *100 to get percentage on each game - on average for the whole bucket


*** the total amount of owners vs the total number of reviews... looking at the number of owners vs their review total

============================  THE QUESTIONS  ============================  


1.	Which games had the most positive reviews and any trends among ownership? What genres and game tags were most popular amongst them? Was pricing a factor? How about languages?

2.	Of those top games, what was the average playtime in the last 2 weeks? Is there a correlation between top games and average playtime in a 2 week period?

3.	Can sale events on Steam effect review count? How about social media?



- other questions to consider with the new api stuff

* publishers and developers that had the most games with the most positive reviews... same with the negative reviews
	* the differences in between pos and neg, who had the biggest gap in between... who had about the same...
* most games fall into the 0 .. 20,000 owner range, why? compare that to game play
* free-to-play games... are there any trends with free games and owners? avg playtime?


I wanted to look at the publishers and developers to see if there was any trends with these and the pricing of games. 


1.	What are the games with the most positive reviews that are free-to-play and pay-to-play? Top developers/publishers amongst those? Top genres? What is the pricing amongst the non-free-to-play games? (I am going to filter for games with at least 500,000 positive reviews for both free and non-free.)
*** maybe people that pay money are more apt to leave reviews... 
*** ratio between pos reviews and paid for games and pos reviews and free games, also the same with negative reviews.



============================  THE START OF THE READ-ME  ============================

Steam was first released on September 12, 2003  [https://www.statista.com/statistics/552623/number-games-released-steam/#:~:text=The%20online%20gaming%20platform%2C%20Steam,gaming%20platform%20in%20the%20world.]

Value started recording gameplay hours in March 2009. [https://skaery.blogspot.com/2009/11/new-steam-community-feature-total.html]

Some older games, one that have been played on Steam prior to March 2009, will be missing data since they didn't start recording gametime play until that time. [https://arstechnica.com/gaming/2014/04/steam-gauge-addressing-your-questions-and-concerns/]

"the only people who show up as "owners" of free-to-play games in our reports are the ones who have downloaded and played those games at least once."


- App_Id: Steam application number
- Name: name of the game
- Developer: developers of the game
- Publishers: publishers of the game
- Score_Rank: score rank based on user reviews
- Postive_Reviews: number of positive reviews
- Negative_Reviews: number of negative reviews
- Userscore: ** come back to this one **
- Owners: number of owners, meaning the number of customers that have bought the license to play the game on Steam
- Avg_Playtime_Lifetime: average playtime in minutes since March 2009
- Avg_Playtime_Two_Weeks: average playtime in minutes since this data was generated (5/26/2024)









====================================================================================   

* things to consider about this dataset
	- when was this dataset created?
	- has it been updated at all?
	- history of Steam itself

Potential questions to ask...

- What are the top 5 highest rated games?
- What are the top 5 highest rated games that are free? ...that are not free?
- Highest ranked games in each genre
- Lowest ranked games in each genre
- Free games in each genre
- Is there a correlation between free games and non-free games and their ratings?
- What about sequel games, like Portal 2? Pricing, rating, genre?
- Release dates... number of reviews
- Controller support vs keyboard only or both?
- different platforms vs free games? non-free games? 
- linux platform that has controller support and multi-player functality? or certain supported language?
- different currencies available on steam? US players vs russian/European?
- initial vs final prices? 
- avg player count on an early access?
- supported languages? which games with more than 30,000 users have multiple supported language?
- avg required hardware across all steam games? avg hardware for mac, windows, linux?

*SteamSpyPlayersESTIMATE - best estimate of total number of people who have played the game since March 2009


1. Does pricing of a particular game have any correlation to the number of players that have played the game over the years?

2. What are the top rated genres through the Steam library and does multiplayer capability have any effect on the rating?

3. How many games offered both keybord and controller support? 

-- additional questions....
 A. how many games were released per year from the beginning of the dataset until the latest? 

B. top rated games by Metacritic, number of players, and what were their platform availabiltes?


-- difference in players and owners, what are the metrics?

** How many games are owned, never played (CCU)? 
** How many games have less than an hour of actual playtime?



============================ RANDOM NOTES AS I GO ALONG ============================

-- there are over 48,000 games with less than 20,000 owners, but they have the highest total averaged lifetime play. Why???
	* maybe because there is more games downloaded than the other categories making the 
	total numbers of minutes greater than the other groups.
	* more games means more mintues played on average regardless of how LONG they played
	the game for.

-- When I pulled this data, it was Memorial Day weekend! So a lot more people could have been online due to being off for the holiday, at least in the US. This data will be a bit obscured due to that but instead of running 73 API's again at a different time, we can take this data and use it as a means to see what Steam is like on a holiday weekend. I may pull API data for certain games...

-- maybe code to find games that have sequels? Like Alien Swarm and Alien Swarm: Reactive Drop

-- after Steam Replayability Sale: how many games have retained players?

-- Games pulled from Steam (featured on front page of Endlessly Replayable)
	Hades 2
	Hades
	Balatro
	Rabbit and Steel
	Noita
	Lethal Company
	Vampire Survivors
	Risk of Rain 2
	The Binding of Isaac: Rebirth
	The Binding of Isaac: Repentence
	Inscrytpion
	Manor Lords


RESOURCES:

https://store.steampowered.com/news/app/304930?updates=true&emclan=103582791435641360&emgid=4183359634549047620  - Unturned had an update around the time I pulled my data






















