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
<img align="center" src="images/Rating_321_Films.png"><br>
Let's see how the distribution of box office earnings are for each rating.
<img align="center" src="images/Ratings_v_Box_Office_Earnings.png"><br>
Even though the R rating is more popular in our data set, PG-13 dominates in overall earnings.<br><br>

Higher earning movies were rated PG-13. This is why our first bar graph shows more R-rated movies, but our second stacked-bar graph shows more earnings for PG-13.<br><br>
From the data we were given, our recommendation is to make a movie with a PG-13 rating.<br>

### Genre
Now, our next question would be which genres are popular in PG-13 movies?<br><br>
With the data we used to find which movie rating showed highest earnings, we will select all the genres that have PG-13 ratings.<br>
<img align="center" src="images/Genres_PG_13.png"><br>
After counting the number of each genres, we created a bar graph to show the top 4 genres that are popular in PG-13 movies
<img align="center" src="images/Top_4_RT.png"> <br>
As you can see, Drama, Comedy, Adventure, and Action genres are the top 4 genres that are popular in PG-13 movies.<br><br>

### Production Budget
Now, with our top 4 popular genres, we want to see how much Microsoft should spend on each genre to return the best profit.<br><br>
We see that most of our data falls in the range of about 20 million to 80 million. 
<img align="center" src="images/filtered_df_boxplot.png"> <br>
We divided our dataframe using the genres' budgets' Inter-Quartile Range (IQR): below the 25th percentile, between the 25th-75th percentile, and above the 75th percentile.<br>
<img align="center" src="images/Three_Data_Frames.png"> <br><br>
Let's see the correlation table for each range (in ascending order).
<img align="center" src="images/Corrs&#32;for&#32;Jupyter.PNG"> <br>
We see that the high-budget dataframe has the best correlation from budget to profit/profit margin.<br><br>
Because the dataframe has a skew, we will look at the median budget values for each genre.<br>
We'll analyze the best budgets to use for the respective genres in this dataframe.
<img align="center" src="images/Top_4_Medians.png"> <br>
The above graph shows the median range of 120 million to 150 million for the top-4 genres' production budgets.<br><br>
## Conclusion
After analyzing our data, we recommend:
* Rating: PG-13
* Genres for PG-13 Movies: Drama, Comedy, Adventure, Action
* Budget: $120,000,000 - $150,000,000
<br>
There is still data to be analyzed, but this would be a good starting point for Micrsoft's film studio.