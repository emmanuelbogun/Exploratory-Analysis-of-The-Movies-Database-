# TMDb Movie Data Analysis
This is my first project of the Udacity's Data Analyst Nanodegree. 

## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#wrangling">Data Wrangling</a></li>
<li><a href="#eda">Exploratory Data Analysis</a></li>
<li><a href="#conclusions">Conclusions</a></li>
</ul>
<a id='intro'></a>

## Introduction
>In this project we'll be analyzing a movies dataset from Kaggle which contains basic information provided by The Movie Database (TMDb) about movies, its popularity, budget, revenue amongst others spanning from 1960 to 2015.
>After data preparation, the characteristics of movies are investigated in respect to the **revenue**, **popularity**, **runtime** and **vote_average**.

### Dataset Description 
>This dataset contains information about 10,000 movies collected from The Movie Database (TMDb). It contains twenty-one (21) columns and below are the descriptions for each  column.
#### Column Description:
**`id`** **`imdb_id`** : unique id or imdb for each movie on TMDB.
<br>**`popularity`** : this measures how popular the movie is.</br>
<br>**`budget`** : the total budget of the movie in USD.</br>
<br>**`revenue`** : total revenue of the movie in USD.</br>
<br>**`original_title`** : the title of the movie.</br>
<br>**`cast`** : names of the cast of the movie separated by "|".</br>
<br>**`homepage`** : the website of the movie.</br>
<br>**`director`** : the name of the director(s) of the movie, it's also separated by "|" when more than 1.</br>
<br>**`tagline`** : a catchphrase describing the movie.</br>
<br>**`keywords`** : keywords related to the movie.</br>
<br>**`overview`** : summary of the plot of the movie.</br>
<br>**`runtime`** : total runtime of the movie in minutes.</br>
<br>**`genre`** : genres of the movie separated by "|".</br>
<br>**`production_companies`** : production company/companies of the movie.</br>
<br>**`release_date`** : release date of the movie.</br>
<br>**`vote_count`** : number of voters of the movie.</br>
<br>**`vote_average`** : average user rating of the movie.</br>
<br>**`release_year`** : release year of the movie ranging from 1960 to 2015.</br>
<br>**`budget_adj`** : the total budget of the movie in USD in terms of 2010 dollars (accounting for inlation over time).</br>
<br>**`revenue_adj`** : the total revenue of the movie in USD in terms of 2010 dollars (accounting for inlation over time).</br>

### Question(s) for Analysis
> #### 1. What genres are the most popular? What is the popularity trend by year?
> #### 2. Do movies with longer duration have higher rating than the short ones?
> #### 3. What features are associated with generating higher revenues?
