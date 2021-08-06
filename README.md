# Movie Analysis
<img align="center" src="images/movie_picture.png"><br>

## Overview
This project will analyze what types of films are currently doing the best at the box office to help Microsoft decide what type of films to create. <br>

## Business Problem
### What is the best type of movie to make for maximum profit?
We each looked at what aspects of a movie will make maximum profit.
* Parental Ratings that give best return 
* Popular Genres
* Production Budget

## How to choose which movie to create <br>

### Rating
We selected all the movie ratings from the data table and counted each ratings. We, then, dropped all the null data and sorted the movies by box office.<br>
<img align="center" src="images/Distribution&#32;of&#32;Ratings.png"><br>
Let's see how the distribution of box office earnings are for each rating.
<img align="center" src="images/Stacked&#32;Bar&#32;Chart.png"><br>
Even though the R rating is more popular in our data set, PG-13 dominates in overall earnings.<br><br>

From the graphs above, lower the earnings are, the most rating of the movie was R-rated. Higher earning movies was PG-13. This shows why our first bar graph showed more R-rated movies but our second stacked-bar graph showed more earnings for PG-13.<br><br>
From the data we were given, our recommendation is to make a movie with the PG-13 rating<br>

### Genre
Now, our next question would be which genres are popular in PG-13 movies?<br><br>
With the data we used to find which movie rating showed highest earnings, we will select all the genres that have PG-13 ratings.<br>
<img align="center" src="images/Genres_PG_13.png"><br>
After counting the number of each genres, we created a bar graph to show the top 4 genres that are popular in PG-13 movies
<img align="center" src="images/Top_4_RT.png"> <br>
As you can see, Drama, Comedy, Adventure, and Action genres are the top 4 genres that are popular in PG-13 movies.<br><br>

### Production Budget
Now, with our top 4 popular genres, we want to see how much Microsoft should sepdnt for those genres to get the best profit.<br>
We see that most of our data falls in the range of about 20 million to 80 million. 
<img align="center" src="images/filtered_df_boxplot.png"> <br>
Let's divide our data into three subsets of datapoints using their budgets' Inter-Quartile Range (IQR): below 25th percentile, between 25th-75th percentile, and above 75th percentile.<br>
<img align="center" src="images/Three_Data_Frames.png"> <br>
Let's see the correlation table for each range.
<img align="center" src="images/Corrs&#32;for&#32;Jupyter.PNG"> <br>
We see that the high-budget dataframe has the best correlation from budget to profit/profit margin.<br>
We'll analyze the best budgets to use for the respective genres in this dataframe.
<img align="center" src="images/High_df_stats.PNG"> <br>
Since the High DF graph above was skewed, we found the median production budgets for each genre from the high-budget (above 75th percentile) dataframe.
<img align="center" src="images/Top_4_Medians.png"> <br>
The above graph shows the median range of 120 million to 150 million for the top-4 genres' production budgets.<br><br>
## Conclusion
After analyzing our data, to make maximum profit movie, we recommend:
* Rating: PG-13
* Genres for PG-13 Movies: Drama, Comedy, Adventure, Action
* Budget: $120,000,000 - $150,000,000