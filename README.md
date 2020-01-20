# Will my new videogame besuccessful ? : a network's perspective

More and more video game platforms are setting a principle of physical dematerialization of games that are now only accessible via download on an online portal.One of these platforms is Steam.  Steam is a video game digital distribution service launched as a standalone software client which provides automatic updates for their games.  It is today the largest digital distribution platform for PC gaming with over a billion registered accounts with 90 million monthly active users.  But each game has its own parameters and thus its own success.What  parameters  influence  the  most  its  popularity  ?This question is indeed quite interesting because today’s video game success may depend also a lot on the review that similar games receive from their platform.  We shall then try to answer this question among others.In this project, we will attempt to find a way to estimate the success or failure of a released game according to different factors such as the category the game belongs to, its price, the gameplay average time, the release date.  In order to do so, we have scrapped our way through steam to gain a bit of knowledge.

# Organisation

This project is organised in 5 different jupyter files and 3 folders:

## Folders

- images : picture of the graphs that we are using during our study.

- data : folder containing the data that we have been parsing and cleaning for our study. It contains:
        - Download : Raw data parsed from Steam and SteamSpy (actually empty due to the large size of the data. Can be collected via 1-data-collection.ipynb)
        - Export : pre-cleaned and processed data

- graphs : folder containing the graphs that we have used to perform our analysis.

- images : images used in the jupyter notebook.


## Jupyter notebooks

1 - Data-Collection: Parser that is parsing the Steam and Steamspy website via dedicated API (If you do not want to parse the data do not use it [it takes ~14h] ). 

2 - Data-cleaning-steam: File used to clean the collected data from the steam API (You need to parse the data).

3 - Data-cleaning-steam: File used to clean the collected data from the Steamspy API and merge the data together with the cleaned steam data (You need to parse the data).

4 - Exploration : Study of the data to understand how the video games on steam are organized, what are the most significant categories, etc... (Data available)

5 - Exploitation : Graph study of the cleaned data via [Gephi](https://gephi.org/) and clustering of the values (Data available).


## Disclaimer

 The data parsing and processing part was greatly inspired by the work of [Nik Davis](https://nik-davis.github.io/posts/2019/steam-data-collection/), original creator of the Steam dataset on [Kaggle](https://www.kaggle.com/nikdavis/steam-store-games). We decided to parse the data by ourselves to have recent data and also to be able to fetch some information not available in the dataset due to the cleaning step.

## Important if you want to study the steam dataset in your country:

The Steam API gives us data about the games that are actually available from the country where you are parsing the data. Hence, parsing from a different country means that the currency, actual number of game available, etc... can be variable. 
