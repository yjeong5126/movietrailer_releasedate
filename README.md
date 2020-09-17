# Analysis of Movies and their Trailer Release Dates
> This is the analysis about the movie release dates and the official trailer release dates. 

## The Goal of this Project
<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/promotion_period.JPG" width="500" height="300">

Let’s define the **Promotion Period** as the period between the *official movie trailer release date* and the *movie release date*. 

<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/promotion_days_distribution.PNG" width="500" height="300">

The graph above shows the distribution of the promotion period for the movies released in the US between 2017 and 2019. As seen in the graph, there is a large variation in the promotion period. 

This project is to examine whether the variation in the promotion period is one of the strategies for promoting the movies. To test this, I examine the factors related to the decision about the length of the promotion period. The factors to be tested are **budget**, **distributors**, **MPAA**, and **genres**. 

## How to Run this Project
Basically, the code for this project is written in the Jupyter Notebook for Python. Therefore, 
- Install Python 3.
- Install Jupyter Notebook.
- Install the Python requirements with pip install -r requirements.txt.
- Open `boxoffice_trailer.ipynb` in the Jupyter Notebook and run the cells.

## Data 
I scraped the two movie websites: 1) boxofficemojo.com and 2) traileraddict.com. The former one provides general movie information for each movie. The latter gives information about dates for each trailer for movies. 

The general method of scraping these information is explained in this link: https://github.com/yjeong5126/scraping_boxofficemojo

The movies used for this analysis played in 2017~2019 in theaters. The total numbers of movies scraped from the boxofficemojo and the traileraddict are 2,711 and 25,047, respectively.

## Findings
### Distributors
<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/distributor_promotion_days.PNG" width="500" height="350">

The promotion period for the major distributors is generally greater than those for the minor distributors. This implies that the size of the distributors is related to the length of the promotion period.

### Budget
<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/budget_promotiondays.PNG" width="500" height="300">

The graph above slightly reveals the positive relationship between budget and the promotion period. This positive relationship becomes stronger as the size of distributors is bigger. 

### MPAA
<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/mpaa_promotion_days.PNG" width="700" height="300">

the distributions of the promotion period are likely to be correlated to MPAA when it comes to between ‘PG-13’ (or ‘PG’) and ‘R’.

### Genres
<img src="https://github.com/yjeong5126/movietrailer_releasedate/blob/master/images/genres_t_ks.PNG" width="400" height="600">

The t-statistics and KS-statistics for some genres are significant. Especially, the distributions of the promotion period for the movies with Action, Adventure, Sci-Fi, Fantasy, Family, or Animation are relatively long compared to other genres.



