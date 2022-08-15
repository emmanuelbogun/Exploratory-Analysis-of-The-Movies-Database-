# TMDb Movie Data Analysis
This is my first project for the Udacity's Data Analyst Nanodegree. The of the project aim is to carry out an investigation which analyzes at least one dependent variable and three independent variables.
# Dataset Description
In this project we'll be analyzing a movies dataset from Kaggle which contains basic information  about 10,000 movies collected from The Movie Database (TMDb) about movies, its popularity, budget, revenue amongst others spanning from 1960 to 2015. This dataset contains twenty-one (21) columns and below are the descriptions for each column:
><br>**`id`** **`imdb_id`** : unique id or imdb for each movie on TMDB.
<br>**`popularity`** : this measures how popular the movie is.
<br>**`budget`** : the total budget of the movie in USD.
<br>**`revenue`** : total revenue of the movie in USD.
<br>**`original_title`** : the title of the movie.
<br>**`cast`** : names of the cast of the movie separated by "|".
<br>**`homepage`** : the website of the movie.
<br>**`director`** : the name of the director(s) of the movie, it's also separated by "|" when more than 1.
<br>**`tagline`** : a catchphrase describing the movie.
<br>**`keywords`** : keywords related to the movie.
<br>**`overview`** : summary of the plot of the movie.
<br>**`runtime`** : total runtime of the movie in minutes.
<br>**`genre`** : genres of the movie separated by "|".
<br>**`production_companies`** : production company/companies of the movie.
<br>**`release_date`** : release date of the movie.
<br>**`vote_count`** : number of voters of the movie.
<br>**`vote_average`** : average user rating of the movie.
<br>**`release_year`** : release year of the movie ranging from 1960 to 2015.
<br>**`budget_adj`** : the total budget of the movie in USD in terms of 2010 dollars (accounting for inlation over time).
<br>**`revenue_adj`** : the total revenue of the movie in USD in terms of 2010 dollars (accounting for inlation over time).

# Questions for Analysis
After data preparation, the characteristics of movies are investigated in respect to the **`revenue`**, **`popularity`**, **`runtime`** and **`vote_average`**. To achieve that the following questions will be answered in this analysis:
<br>**1. What genres are the most popular? What is the popularity trend by year?**
<br>**2. Do movies with longer duration have higher rating than the short ones?**
<br>**3. What features are associated with generating higher revenues?**</br>

# Importing the necessary packages
The following libraries were imported:
- **Pandas** for data wrangling, cleaning and exploration.
- **NumPy** for numerical and mathematical computations.
- **Matplotlib** for creating interactive visualizations.
- **Seaborn** to improve the quality of the visualiztions.
- **%matplotlib inline** magic function to enable inline plotting. 

# Data Wrangling
Here we'll be loading our data and checking for its general properties to get a better understanding of the data. To do this, we'll be checking for the:
- shape of the data
- data type of the columns
- columns containing missing values
- descriptive statistics of the columns

**Some quick findings from the summary statistics:**
- Some rows of the **runtime** column contain 0, which is quite abnormal because a movie can't have a runtime of 0 minutes.
- At least 50% of the values in the **budget** and **revenue** columns contained 0.
- Majority of the movies were released between **1995** and **2011**.
- Suspected presence of outliers in the **popularity** and **runtime** columns.

**Data Cleaning**
> Here we'll be checking for:
- duplicate rows and dropping them.
- fixing data type of columns in wrong format.
- dropping the rows in the columns containing zeros.
- creating new columns.
- dropping unwanted columns.

# Conclusions
- Higher budgets and popularity were **positively correlated** to Higher Revenue. This is quite explainable, assuming that a higher budget for promotions and advertisements will increase the popularity of the movie. This in turn will led to generating higher revenue for the movie.
- Also the duration of the movies, either short or very long **did not affect** the average user rating of the movies.
- Over the years, there was an **increase in trend** for the general popularity of movies.

# Limitations
- At least 50% of the data for both the revenue and budget columns were dropped as they contained zeros. So this analysis was performed with a few part (only **3849 rows and 14 columns**) of the original dataset.
- Popularity and the runtime columns contained **outliers** as seen from the descriptive statistics.
- The movies has multiple values for genres, casts and directors. We kept only the first names while others were dropped.
- Hence, some of the assumptions here may not be applicable to the original dataset.
