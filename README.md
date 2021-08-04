# Movie Analysis
<img align="center" src="images/movie_picture.png"><br>

## Overview
This project will analyze what types of films are currently doing the best at the box office to help Microsoft decide what type of films to create. <br>

## Business Problem
### What is the best type of movie to make for maximum profit?
We each looked at what aspects of a movie will make maximum profit.
* Correlation of budget and profit margin
* Popular Genres
* Parental Ratings that give best return 

## How to choose which movie to create
### Budget vs. Profit Margin
#### If Microsoft spends x amount more, will profits increase by y?
First, we filtered out movies that was release before 2005 to get approximately 10 years worth of data. 
Since the range of the production budget was big, we created a box plot to see which range of budget we should use to analyze.<br>
(box plot)<br>
After looking at the box plot above, we decided to separate movies in 3 different ranges: below the 25th percentile, between the 25th and the 75th percentile, and above the 75th percentile to see correlation of budget and profit margin.
With our filtered data, now we asked ourselves: for Microsoft to enter the film industry, what's a good production budget?<br>
(low corr scatter plot)<br>
(low corr data table)<br>
As you can see in the scatter plot and the data table, data below the 25th percentile has very slight positive correlation of 0.009746 between the produciton budget and the profit margin.<br>
(mid corr scatter plot)<br>
(mid corr data table)<br>
As you can see in the scatter plot and the data table, data between the 25th and the 75th percentile has very slight positive correlation of 0.091774 between the produciton budget and the profit margin but it is higher than the low budget data.<br>
(high corr scatter)<br>
(high corr data table)<br>
As you can see in the scatter plot and the data table, data above the 75th percentile has very slight positive correlation of 0.208846 between the produciton budget and the profit margin but it is higher than both low budget and mid budget data.<br>
With the analyzed data from above, we can conclude that, on average, a higher budget will lead to a larger profit, and will likely lead to a higher profit margin.

### Genre
After sorting the movies using profit and net margin profit (over 70%), we took the genres from each movie and created bar graph to show popular genres in a movie that profited the most. 
This bar graph shows set of genres that are popular for each movie that profited the most.<br>
<img align="center" src="images/set_of_genres_top_100_profited_movies.png"><br>
You can see that "Action, Adventure, Sci-Fi" and "Adventure, Animation, Comedy" are the most popular set of genres for movies.
Then we took the sets of genres and separated them individually to create a bar graph of each genres that are popular for each movie that profited the most.<br>
<img align="center" src="images/genres_in_top_100_profited_movies.png"><br>
You can see that Adventure, Action, Comedy, Animation, and Sci-Fi were top 5 popular genres.<br>

### Rating
We selected all the movie ratings from the data table and counted each ratings. We, then, dropped all the null data and sorted the movies by box office.<br>
First, we created histograms to show the top 105 ratings in box office and bottom 105 ratings in box office.<br>
<img align="center" src="images/Top&#32;105&#32;Box&#32;Office.png"><br>
<img align="center" src="images/Bottom&#32;105&#32;Box&#32;Office.png"><br>
As you can see, PG-13 movies profited the most while R-rated movies profited the least.<br>
We want to

## Conclusion