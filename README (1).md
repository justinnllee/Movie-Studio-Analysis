
# Movie Studio Analysis

Justin Lee

This notebook is prepared for Electronic Arts (EA), a company renowned for producing video games. EA has observed that many major companies are now creating original video content and is keen to enter this market on a global scale. EA seeks three business recommendations on the types of films to produce.



## Business Understanding
The company requests that the focus be solely on animated movies, as it aligns with their expertise in video game production. For this analysis, we will consider only movies with a rating above 7.5, as this represents the minimum quality standard EA aims to achieve. Additionally, the analysis will be based on data from countries with at least thirty movie premieres in a given region.
## Data Understanding
This data is from IMDb that includes movie data. Each movie has a unique ID associated with it that contains its title, start year, runtime and genre. The movie ID associated with it also links it to its average rating, number of votes received, region and languaged it aired in, and other data such as directors, writers, and other principals. The three main tables we will use for our analysis are movie_ratings, movie_basics, and movie_akas. Each table's columns can be shown below.

Some initial limitations in this dataset include missing/NaN values. I will remove these NaN values from my dataset.
## Data Preparation
To filter my data to my stakeholder's specific requests, I've created different dataframes for each business recommendation.

First I broke up different runtime (in minutes) dataframes and removed all NaN values. I created four different dataframes to break up runtime between 30 to 60 minutes, 60 to 90, 90 to 120, and 120 to 150.

Second, I created a new dataframe just to showcase animation movies with their total average rating. I also only showcased data that had a rating above 7.5 as per our client's request. To make it easier to read, I've ordered the data in descending order.

Third, I created a new dataframe that showcased the number of regions with the lowest average votes, and to make it easier to read I've ordered the data in asecnding order. This data is also filtered by having at least thirty movies aired in a given region as per our client's request.
## Exploratory Data Analysis
These visualizations will help to support our three business recommendations. From these visualizations we can determine the best runtime in minutes, which animation movie genre typically performs the best, and which global regions we should avoid airing movies in based on vote count.
## Conclusion
This analysis leads me to three recommendations for Electronic Arts (EA) to enter the movie creation space.

1) Create movies that have runtimes between 30-60 minutes. Compared to other runtimes, movies from this dataset and runtime length typically scored the highest average rating.

2) Create "Animation, Fantasy" movies. Of all Animation genres, the "Animation, Fantasy" movies scored the highest average rating.

3) Avoid airing movies in Nepal, Nigeria, Morocco, Iraq, Mongolia, Palestinian Territory, Tunisia, Pakistan, Belarus and Algeria as these ten regions scored the lowest on average votes of regions where at least thrity movies aired.
## Limitations and Next Steps
Some limitations arose from my analysis and the way I manipulated the dataframes to support these business recommendations.

1) These dataframes were created based on conditions on each of their respective recommendations, but is not filtered for all three prompts. For example, in selecting which regions had the lowest amount of votes - these were lowest votes across all genres instead of just Animation movies. Nepal could have the lowest amount of votes across all movies, but could perform better in Animation genres compared to other regions. The next step would be to create an analysis specific to all conditions of my client.

2) This data had missing NaN values. For my analysis, I've just excluded these values. If we had a value for these NaN values we could have led to a more accurate conclusion. A next step would be to obtain values for these missing NaN values to perform a more accurate analysis.

3) This data is only inclusive of IMDb data. There are tons of other movie datasets out there and of different genres, years, scoring systems, etc. To give my client more well-rounded business recommendations, the next stpe would be to create an analysis across different types of movie data.