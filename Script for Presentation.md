OPENING:
Hi there! My name is Barb and I will be presenting today my analysis on data I collected from the pc-gaming platform, Steam.

----------------------------------------------------------------------------------------------

INTRO SLIDE:
So what exactly is Steam? It was first launched in the Fall of 2003 by a video game developer named Valve Coropartion as a way to automatically provide game updates for its current games at the time. 

In November 2004 the first game was release on the platform for digital download.

By 2005, multiple third-party developers had contracts to release their games on Steam.

Over the years, Valve has released numerous games as both a developer and a publisher and has acquired 1000s of other games on their platform. Now they are the definitive PC-gaming platform!

Why did I choose Steam data for my analysis? Well first and foremost, I love video gaming! So I thought why not explore data on something that is a big part of my life. I thought it would be cool to see some behind-the-scene data that helps make up its platform. And maybe help a fellow gamer find a cool new game to try in the process. Or even help a Developer or Publisher see the truth about their games.

How did I get all this data? I ran over 100 API calls to a partner website called SteamSpy to retrieve the entire gaming collection that makes up Steam. I took those json files, converted them all to csv's, imported into Python, and away I went!

My main takeaway from this was to see the following:
- what are the top games that are in the Steam database based on positive reviews from its players? Are there any trends associated with these games? What are the different gamer tags, genres, and supported languages associated with these games? 

- Can social media affect review count over time?

I am hopeful to extract these points from the analysis ahead!]]

----------------------------------------------------------------------------------------------

INFO SLIDE:
Now I began my analysis. An overall look at it gave me some very interesting numbers. As you can see, there are…

- Over 70 thousand games currently active on Steam
- Almost 44 thousand developers and a little over 38 thousand publishers tied to those games
- 125 million total reviews through the games and over 600 thousand of playtime minutes
- Sum of all the game prices total to over half a million dollars
- 13 different owner buckets, which I will explain later
- and over 8 million users playing games across Steam at one given time!

----------------------------------------------------------------------------------------------

POSITIVE/NEGATIVE REVIEWS:
This first dashboard shows us the positive and negative reviews across the Steam library. I have broken them down into Free-to-Play games vs Pay-to-Play games and Developer vs Publisher. 

As you can see the free-to-play games tend to have higher reviews overall than the pay-to-play games, meaning the highest positive reviewed free game is Counter-Strike: Global Offensive at just over 7 million while the highest positive reviewed paid game is just over 1.5 million.

The Developer and Publisher charts overall looked similar with a few outliers here and there. 

Also to keep something in mind, 67.5% of games are developed and published by the same company where as 32.5% have differing developers and publishers. This dashboard reflects that as well!

[click on COUNTERSTRIKE POS REVIEWS to show it interacting] - as you can see, this shows the 7 mil positive reviews with over a million negative reviews and how it has the same Developer and Publisher VALVE - [unclick POS REVIEW]

HOVER OVER GTA TO SHOW POSITIVE REVIEWS

Alternatively you can interact with the scatters on the bottom to see the games for each catergory. [click TOP BLUE DOT CHOICE OF GAMES] as you can see it showing that this developer also publishes it's own games and has nothing but pay to play games while [click TOP PINK DOT BIG FISH] Big Fish games has both multiple developers and games that are pay to play AND free to play.

----------------------------------------------------------------------------------------------

DEV/PUB INFO:

Next we are going to dive deeper into the Developers and Publishers for the Steam database. I decided to focus on the top 5 for this dashboard. The top 5 was based on the total number of positive reviews for each Developer and Publisher. This one is made to be interactive, lemme show you!

The bar charts are showing the average price in each owner bucket per Dev or Publisher.

The pie charts are breaking down the total game play for each dev and publisher within the last 2 weeks and peak online players at one time playing their games.

[click on YELLOW BUCKET 2ND FROM TOP] - on average games developed by CAPCOM that have between 2 Million and 5 Million owners have an average game price of $33, have played over 2,000 mins and over 41,000 players were online at the same time playing their games. [unclock YELLOW BUCKET ON GRAPH]

[click on SAME YELLOW BUCKET 3RD FROM TOP] - looking at the same owner bucket we see that games published by Electronic Arts have an average of $23 in game price, have played over 2,000 mils but had almost 100,000 players online at the same time playing their games. [unclick YELLOW BUCKET or click on heading...]

Now, you can choose to pick an owner bucket as well. If we were to look at data from the games that had 50 THOUSAND TO 100 THOUSAND, you can see how it interacts along with each top 5 developer and publisher.

----------------------------------------------------------------------------------------------

OWNERS:
Next, I'm going to show you the Owner bucket dashboard!

So what exactly does "Owner" bucket mean? On Steamspy, where I ran the APIs, owners is classifed as an owner of a particular game. Simply put, this account or player has this game in their library where say they downloaded it from Steam itself or went to a store like GameStop and retrieved a Steam key for download, etc. Either way they now "own" this game. 

SteamSpy put the Owners into groups or what I like to call "buckets". There are 13 total buckets ranging from 0 - 20,000 owners to 100 million - 200 million owners PER GAME. 

So this dashboard is breaking down all the metrics by Owner bucket. The top left graph is showing TOTAL POSITIVE REVIEWS across all user buckets. The top right is showing the AVERAGE PERCENTAGE of positive reviews per owner bucket. The bubble chart is showing the average discounts across the owner buckets. And lastly the tree maps across the bottom of the dashboard are showing the average price, gameplay within the last 2 weeks, and peak online players all per owner bucket.

[click on YELLOW DOT - TOTAL REVIEWS] - this owner bucket of 2 million to 5 million has the most TOTAL positive reviews across all buckets with an average discount of 10%, average price of $16.67, over 130 thousand gameplay mins, and over 1 million players online at the same time playing those games. [UNCLICK YELLOW DOT TOTAL REVIEWS]

Next I wanted to look at the percentage of positive and negative reviews. If we look at the top bucket [CLICK ON RED DOT] we see that actually the owner bucket of 20 million to 50 million on average had the highest positive review percentage at 87.7%. It averaged about 4.5% in discounts, averaged $15 in game price, 22,000 gameplay mins in the last 2 weeks, and over a million players online playing those games.

I feel like positive reviews can play a huge part in deciding on a particular game to play, just like searching for at least 4 star reviews on Amazon!

I dove deeper into this owner bucket with my next dashboard.

----------------------------------------------------------------------------------------------

20-50 MIL DATA:
Let's look at that top owner bucket. As you can see to the left I have listed out the 24 games found in that owner bucket. We also have the top 25 most popular gamer tags, total gameplay, pricing per game, percentages of positive vs negative reivews, genres, supported languages, and their developer and publisher.

Let's look at the Top Free to Play game and Top Pay to Play game.

[click on UNTURNED NAME] - Lets look at UNTURNED. It has several of the top gamer tags listed, almost 3 thousand mins in gametime play, blank means it's free, 91.5% positive review rating, multiple genres, and developed and published by the same company Smartly Dressed Games. It's only con is it has just the one supported language which may hinder it's access across the world.

Next Let's look at Stardew Valley. [CLICK ON NAME] - It has multiple gamer tags among the top 25, almost 7 hundred mins of game play, $14.99 for the game, genres include Indie/RPG/Simulation, multiple supported languages and ConcernedApe as both Dev and Publisher. This has the highest positive review rating out of our games!

----------------------------------------------------------------------------------------------

SUMMARY:
So what did we notice in our data??

Top free-to-play game with the most positive reviews was Counter Strike Global Offensive 

Top pay-to-play game with the most positive reviews was Grand Theft Auto 5.

The top Developer was CAPCOM and the top publisher was Electronic Arts, both based on total positive reviews.

The top owner bucket based on percentage of overall positive reviews was 20 to 50 million owners.

The top free to play game in that bucket was UNTURNED. 

The top pay to play game in the bucket was Stardew Valley.


Based soley on Developer and Publisher, any games developed by CAPCOM or published by Electronic Arts would be good to check out.

As far as our top owner bucket with 20 million to 50 million owners based on percentage of positive reviews, any of those games I would recommened to check out! Especially Stardew Valley with having a 98% percentage positive review rating overall!

Since I have emphasized how important reviews can be in video games, I decided to dive a little further into this with a game in particular.


----------------------------------------------------------------------------------------------

TEAM FORTRESS 2:
There is a game on Steam that has been around since 2007 that is actually a product of Valve itself. I am talking about Team Fortress 2.

Since the beginning of June there has been a website called save.tf. Quoted from their website, the game’s official servers have been overrun by hordes of cheating aimbots while Valve has remained steadfast in their refusal to adequately tackle the problem.

So the people behind the website of added a petition for people to sign to try and get Valve's attention. So far they have over 300 thousand signatures. 

I decided to run API calls each day for 11 days to track the positive and negative reviews. As you can see, there have been almost 6 thousand LESS positive reviews (meaning players have removed their inital positive reviews) and there have been almost 18 thousand negative added to the game on Steam.

So this is a visualization that social media CAN make an impact on reviews!!

----------------------------------------------------------------------------------------------

CLOSING:
Here are some sources I used in my presentation. Thank you! Are there any questions?

