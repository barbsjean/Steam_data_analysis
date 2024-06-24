![image](https://github.com/barbsjean/Steam_data_analysis/assets/156152785/c16f120c-b76c-4ad1-a9cb-9cb0ae60c867)


# Steam Data Analysis

_My Capstone project for the Data Analytics Cohort #11 at Nashville Software School_

## I decided to do my Capstone on data I acquired from the pc-gaming platform, Steam.

### What exactly is Steam?

Steam was first launched in the Fall of 2003 by Valve Coroporation as a way to automatically provide game updates for its games at the time. By November of 2004, they released their first game for digital download. By 2005, they had multiple third-party developers releasing their games on Steam's playform. Now they are the definitve pc-gaming platform!

### How did I extract all this data?

I ran over 100 API calls to a partner website called SteamSpy to retrieve as much of the gaming collection as I could. I took those json files, converted them all to csv's, imported into Python, and away I went! 

I used the following technologies:
* [SteamSpy's Api](https://steamspy.com/api.php) - for all of my API calles
* Postman - used this mainly for the API calls themselves, from here I saved them each into a csv file on my computer
* json2csv - software I downloaded to convert each csv to a json file
* Python - imported all csv's directly into Python for viewing
* Tableau - what I used to create my presentation and dashboards of my data

From the data I pulled there was over 70,000 active games, a total of over 80,000 developers and publishers tied to those games, and over 125 reviews submitted by Steam players. 

### Why did I decide on this kind of data?

Simply put, I love to video game! It's one of my main hobbies and a way for me to unwind, recharge and relax. Another reason was to some behind-the-scenes data that helps make up the platform. I also thought it may be useful to a developer or publisher as a way for them to see the truth in their games behind the data.

### My Analyis

What I wanted to find was the following:

1. what are the top games that are in the Steam database based on positive reviews from its players? Are there any trends associated with these games? What are the different gamer tags, genres, and supported languages associated with these games?

2. Can social media affect review count over time?

