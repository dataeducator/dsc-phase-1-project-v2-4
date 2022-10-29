# Microsoft Movie Studios Viability Analysis
***
![My Image](Images/Data_Analysis_Microsoft_Movie_Studios.jpg)
# Overview
Microsoft is uniquely situated to leverage its existing technology holidings to redefine the film industry by crafting a one stop shop platform which manages the entire process from preproduction to filming to distribution. Microsoft's executives are in search of actionable ways to ensure successful movies are produced as they launch a new movie studio that is well supported from its onset. 

# Goals:
The project has the following guiding questions:
* When is the best time of year to release a movie?
    - Find trends in the profit of movies based on their release month among the most profitable movies.
* Which director makes the most profitable movies?
    - Find directors who have proven track record of making films that generate profits worldwide.
* Which genres of movies make the most profit at the box office?
    - Determine pattern among succesful movie launches including the type and time of year they are released.
 
 # Data Understanding
***

The datasets used in this project are from the following sources:
* [IMDB](https://www.imdb.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [Box Office Mojo](https://www.boxofficemojo.com/)
* [The Numbers](https://www.the-numbers.com/)

    
# Method:
***
This project will explore data related to current trends in the movie industry. This exploration will include:
* __Importing Relevant libraries and packages__
    - Access code from different modules
* __Data Preparation__
    - Access databases and dataframes useful to this project
    - Investigate data shape and datatype information
    - Drop or impute null values
    - Reduce complexity (ex. join dataframes where necessary, remove or replace missing values, address duplicates data)
* __Addressing Question 1 through Exploratory Data Analysis (EDA)__ 
    - Build or extract features from cleaned data
    - Make visualizations
    - Analyze correlations
    - Summarize findings
* __Addression Question 2 through EDA__
    - Build or extract features from cleaned data
    - Make visualizations
    - Analyze correlations
    - Summarize findings
* __Addressing Question 3 through EDA__
    - Build or extract features from cleaned data
    - Make visualizations
    - Analyze correlations
    - Summarize findings
* __Insights & Recommendations__
    - Discuss findings
    - Identify next steps based on findings
    
 # Data Preparation
***
In order to determine answers to my guiding questions, first I needed to import relevant libraries and packages. 

- <code>sqlite3</code>: a library that provides a SQL interface that allows accessing and manipulating SQL database
- <code>pandas</code>: a data analysis and manipulation library which allows for flexible reading, writing, and reshaping of data
- <code>numpy</code>: a key library that brings the computationaly power of languages like C to Python
- <code>matplotlib</code>: a comprehensive visualization library
- <code>seaborn</code>: a data visualization library based on matplotlib 

I used methods like <code>.info()</code>, <code>.head()</code> to review data shape and statistics. I alos used <code>.dropna()</code> to remove missing values from dataframes if that data was less than 1% of the overall data within a column. I replaced values by using a combination of <code>.fillna()</code> and <code>.median()</code> replace missing values with the median value. I combined dataframes using <code>.merge()</code> and <code>.replace()</code>to ensure that dataframe queries yielded results that I could analyze.


# Question 1: When is the best time of year to release a movie?
***
For the first question I looked for correlations between attributes for the most profitable films. I explored data related to this question using visualizations created with <code>seaborn</code> and <code>matplotlib</code>.

## Visualization for Question 1

![EDA_for_Question_1](Images/EDA_for_Question_1.png)

# Question 2:  Which director makes the most profitable movies?
***
For the second question I looked at looked for correlations between the director of a movie and the profit for the top 100 most profitable movies. I explored this question by sorting values in a combined data frame using <cod>.sort_values()</code> along with visualizations created with <code>seaborn</code> and <code>matplotlib</code>

## Visualization for Question 2

![EDA_for_Question_2](Images/EDA_for_Question_2.png)

# Question 3:  Which director makes the most profitable movies?
***
For the second question I looked at looked for correlations between the director of a movie and the profit for the top 100 most profitable movies. I explored this question by sorting values in a combined data frame using <cod>.sort_values()</code> along with visualizations created with <code>seaborn</code> and <code>matplotlib</code>

## Visualization for Question 3

![EDA_for_Question_3](Images/EDA_for_Question_3.png)

# Insights and Recommendations
***
## Insights
After look at relationships between release month and worldwide profit generation I found that the best months to release a movie are May, June, July, November and December. With __May__, __June__ and __July__ (Summer months) yielding the largest profits in the top most profitable films. 
When viewing the top directors of the top 100 most profitable movies, I found that __Joe and Anthony Russo__ directed the most profitable movies out of the top 100 most profitable movies. While Colin Treverrow, James Wan, and Joss Whedon are amongst the top 5 directors to choose from when choosing directors based on their ability to create profitable movies. 
Finally, after looking for patterns between genre and worldwide profit, I found that while __Animation__ is the best genre of movie to make with Adventure, Action, Sci-Fi and Musicals rounding out the top five best genres to create based on worldwide profit. 

## Recommendations
Create movies that are __Sci-Fi, __Animation__ or __Adventure films__ with a budget of approximately 215 million dollars. When creating movies, use effective directors, specially choose a director like *Joe Russo, Anthony Russo, Colin Treverrow, James Wan or Joss Whedon* who have demonstrated successful direction of profitable movies on the worldwide stage.  If the film you launch is in the Sci-Fi genre, release it during May.  If the film you launch is in the Animation genre, launch it during June or July.  If the film you launch is in the Adventure genre, launch it during November. This will allow the new Microsoft studio to diversify their entry into the large video content space as the median worldwide profit for these films was found to be around __$200 million dollars__.

# Future Work
* Gather and analyze data on the genre of movies each director is known for.
* Use webscraping tools like <code>beautifulsoup</code> to find valuable insights from the film ratings and advertising budgets.
 