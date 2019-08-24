# Life Expectancy

In this project, we perform multiple linear regression to find the key features to affect life expectancy in different countries.

## Goal

Finding which public health factors have the most significant impact on life expectancy by country

## Data Sources:

The dataset was was collected from "WHO" and the United Nations website by Deeksha Russell and Duan Wang and is now stored on [Kaggle](https://www.kaggle.com/kumarajarshi/life-expectancy-who "Kaggle"). It contains 2939 observations about different countries between the years 2000 and 2015.

| Data                     | Data                             |
| ------------------------ | -------------------------------- |
| Country                  | HIV\AIDS                         |
| Year                     | Hepatitis B                      |
| Life expectancy          | Polio                            |
| Adult mortality          | Diphtheria                       |
| Infant mortality         | GDP                              |
| Alcohol consumpton       | Population                       |
| Expenditre on hleath (%) | Prevalence for malnutrition 1-19 |
| Measles                  | Prevalence for malnutrition 5-9  |
| BMI                      | Education                        |
| Status                   | Total expenditre on health       |

## Technical Description

To increase collaboration efficiency we created a GitHub repository; this allowed us to work uninterrupted, simultaneously, and independently.

To achieve the goal we utilized, [Pandas](https://pandas.pydata.org/pandas-docs/stable/index.html/ "Pandas") to clean and explore the data. Additionally, we used [Numpy](https://www.numpy.org/ "Numpy"), [Scipy](https://www.numpy.org/ "Scipy"), and [Sklearn](https://scikit-learn.org/stable/ "Sklearn") for data analysis.

To increase collaboration efficiency we created a [GitHub](https://github.com/DaggerForce/Life_Expectancy_Project/ "GitHub") repository; this allowed us to work uninterrupted, simultaneously, and independently.

The majority of our code was written in Jupyter Notebooks using Python. Furthermore, we used [VSCode](https://code.visualstudio.com/ "VSCode") to a module that contains our helper functions

Initially, we assessed which predictors could have the greatest influence on life expectancy from our dataset. Additionally, we created 4 more features that we suspected could affect life expectancy.

1. Population Size - We divided our countries into three catagories; Small, Medium, and Large.
2. Lifestyle - We created an interaction between alcohol consumption and BMI
3. Economy - The interaction between the population and the GDP.
4. Death ratio - The ratio between adult and child mortality.

Despite the fact we had a decent sized dataset, it was largely fragmented. We chose to remove all the fragmented observations for columns we suspected could have a significant effect on life expectancy.

## Workflow

* Raise a question - Which public health factors have the greatest impact on life expectancy by country? 
* Explore the Dataset
  * Add Features
  * Clean the Dataset
* Model
* Test Models
* Predict Life Expectancy
  
## Results

We started out by looking at the distribution of genres within the top rated movies in TMDb. Out of the 1000 highest rated movies 28.8% of movies were tagged as "Dramas".

![Total Movies Per Genre Pie](Images/genre_pie.JPG "Total Movies Per Genre Pie")

Before we dove deeper into more analyses we first tested the two different rating metrics that were available to us (rotten tomatoes rating and TMDB's popularity) with the box office revenues to check which metric correlated better.

<img src=Images/rev_over_popu.JPG alt="[Popularity and Revenues" width="450"/> <img src=Images/rev_over_rating.JPG alt="RT Rating and Revenues" width="450"/>

Popularity correlated better with the average revenues (r=0.7349) than rotten tomatoes rating (r=0.0666). We followed by checking each genre's popularity.

<img src=Images/genre_popu.JPG alt="Revenue per genre chart" width="450"/>

Out of the 18 different tags drama movies were rated the 16th most popular. We continued by looking at the most popular drama movies comparing them to the most popular movies to check whether drama movies are not as good as the most popular ones (subjectively speaking).

<img src=Images/genre_pop_list.JPG alt="Most popular Dramas list" width="450"/>

<img src=Images/top10_pop_list.JPG alt="Most popular movies list" width="450"/>

Subjectively speaking the quality of dramatic cinema does not fall short in comparison to the most popular movies.

Our next step was to check the average revenue for each genre, top 12 directors, and to list the movies that made the most amount of money at the box office to see if there's a common  denominator.

<img src=Images/genre_revu.JPG alt="Revenue per Genre Bar Char" width="450"/>

<img src=Images/top_rev_direct.JPG alt="Revenue for Top 12 Directors Bar Char" width="450"/>

<img src=Images/top_rev_list.JPG alt="Highest Grossing Films List" width="450"/>

In addition to dramas not being most popular they also did not bring in the most amount of money at the box office.  However, we were able to find a possible common denominator between the highest grossing films.

## Take Home Message

This was just an initial scope. Our recommendation is focused more on what content not to create, dramatic cinema. The market is saturated and these movies and those movies are not the most so popular among viewers.

If an immediate decision has to be made, we would recommend filming an action/adventure movie, based on a comic series or book.

