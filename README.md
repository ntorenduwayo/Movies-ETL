# Movies-ETL
## Overview of the analysis<br/><br/>
A client at Amazing Prime Video, a platform for streaming movies and TV shows on Amazing Prime would like our assistance in creating a dataset for a hackathon. There are two data sources: a scrape of Wikipedia for all movies released since 1990, and a rating data from the Movie Land’s website. We will help extract the data from the two sources, transform it in one clean data set, and load it into a SQL table.<br/>
To achieve this task, we will use Python and Pandas to perform data wrangling (i.e., a process of cleaning and unifying messy and complex data sets for easy access and analysis), and PostgreSQL to store our finished data.<br/>
Our work will help the Amazing Prime Video’s hackathon to develop an algorithm to predict which low budget movies being released will become a popular so that the company can buy streaming rights at a bargain.<br/><br/> 
## Results<br/><br/>
### 1.	ETL Function to read data file<br/>
-	We wrote a function *extract_transform_load* to read three data files (i.e., Wikipedia data, Kaggle metadata, and MovieLens Rating data). <br/>For more information see *ETL_function_test.ipynb* file.<br/><br/>
### 2.	Extract and Transform the Wikipedia data<br/>
-	We extracted and transformed Wikipedia data:<br/>
*	We filtered out the TV shows and created a wiki_movies dataframe.<br/>
*	We cleaned the following columns from the wiki_movies dataframe: the box office, the budget, the release date, and the running time columns.<br/>
	For more information see *ETL_clean_wiki_movies.ipynb* file.<br/><br/>
### 3.	Extract and Transform the Kaggle data<br/>
-	We used the ETL function (i.e., *extract_transform_load*) we create earlier to extract and transform the MovieLens ratings data.<br/>
-	We cleaned the ratings counts<br/>
  For more information see *ETL_clean_kaggle_data.ipynb* file.<br/><br/>
### 4.	Movie Database<br/>
-	We used Python, Pandas, PostgresSQL to add movies DataFrame and MovieLens rating CSV data to a SQL database.

