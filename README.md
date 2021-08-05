# Movie Analysis
<img align="center" src="images/movie_picture.png"><br>

## Overview
This project will analyze what types of films are currently doing the best at the box office to help Microsoft decide what type of films to create. <br>

## Business Problem
### What is the best type of movie to make for maximum profit?
We each looked at what aspects of a movie will make maximum profit.
* Parental Ratings that give best return 
* Popular Genres
* Correlation of budget and profit margin

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
<img align="center" src="images/Top_5_RT.png"> <br>
As you can see, Drama, Comedy, Adventure, and Action genres are the top 4 genres that are popular in PG-13 movies.<br><br>

### Budget vs. Profit Margin





## Conclusion
After analyzing our data, to make maximum profit movie, we recommend:
* Rating: PG-13
* Genres for PG-13 Movies: Drama, Comedy, Adventure, Action
* Budget: $115,000,000