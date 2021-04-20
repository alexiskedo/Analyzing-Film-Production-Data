# Microsoft Film Studio: Data Analysis & Strategy Recommendations
### Author: Alexis Kedo
## Overview
This project analyzes selected characteristics of movies produced from 2010 onward, in order to provide a set of recommendations to guide the actions of a corporation, Microsoft, in its goal to open a movie production studio. The data comes from the [Internet Movie Database (IMDB)](https://www.imdb.com/interfaces/), [The Numbers](https://www.the-numbers.com/), [Box Office Mojo](https://www.boxofficemojo.com/), [The Movie Database](https://www.themoviedb.org/?language=en-US), and [Rotten Tomatoes](https://www.rottentomatoes.com/), courtesy of [Flatiron School](https://flatironschool.com/). Descriptive analysis of film release and earnings data shows that a film's popularity varies seasonally and that Microsoft should limit its production efforts to a few genres in order to maximize profitability. Furthermore, a sampling and analysis of most popular actors shows that Microsoft should concentrate their hiring on a select pool of actors who are relatively likely to maximize return on investment. 
## Business Problem 
As a novice entree into the film production industry, Microsoft faces steep competition from a host of more established firms, includng Netflix, Amazon, and Hulu. In addition, Microsoft's primary software competitor, Apple, has been producing its own feature-length content since [2019](https://www.nytimes.com/2019/09/27/business/media/apple-movie-theaters.html). In order to produce movies that can stand up to the output of its competitors, Microsoft will likely need to expend billions in start-up costs, which makes its initial investment decisions especially important. Amazon spent [5 billion dollars](https://www.nasdaq.com/articles/does-amazon-profit-its-original-tv-shows-movies-2018-03-15) on "original programming" in 2018, while Netflix spend $8 billion. 

While most pre-production costs (e.g. insurance, equipment rental, crew staffing costs) are more or less fixed, "above-the-line"  (i.e. creative) costs can vary widely. As actor salaries constitute [a significant](https://www.forbes.com/sites/schuylermoore/2019/04/13/the-importance-of-film-budgets/?sh=2df1507727f5) portion, it makes sense to concentrate part of this analysis on on-screen talent. Release month is also a major decision point around which there has been [some](https://www.newyorker.com/magazine/2015/02/23/rethinking-seasonal-strategy) questioning of the traditional strategy of releasing blockbusters over the summer and prestige films prior to awards season. Finally, the all-important question of what genres will generate the most return on investment is a debate that [continues](https://grayll.medium.com/the-most-profitable-film-genres-e91d5fb4cfa5) to [rage](https://www.mentalfloss.com/article/68552/20-most-profitable-movies-all-time-based-return-investment). For these reasons, I have concentrated my analysis on these three major areas. 
## Data
As stated above, datasets were pulled from a variety of online sources. IMDB datasets were the most used files in this analysis and provide unique IDs for both movies and actors. IMDB files also supply various characteristics about movies (start year, genre) and actors (birth year, death year, average ratings per movie). The "budgets" dataset from The Numbers was also used to provide gross worldwide earnings information. The sample included movies released after 2010. Actor data was narrowed to include only actors born after 1940.

The three main decision-making areas addressed by this project were release month, genre, and available actors. The target variables for anlysis were average popularity (used for both seasonality and actor analysis), average worldwide gross earnings (used for genre analysis), average ratings per movie (used for actor analysis), and net worth (used to create a scale to represent the approximate 'cost ' of hiring a particular actor).
## Methods
This project uses descriptive analysis, including description of trends over time, aggregating data across categories, and sampling. These methods allows us to gain insight into some potential opportunities for a start-up studio to gain a foothold in a competitive industry. 
## Results

![months](https://user-images.githubusercontent.com/77643869/115327838-406b5480-a155-11eb-8987-ef54ffe8b5af.png)

Movies with peak average popularity are released during the peak "cluster" months of June, July, November, and December, though there is also above-average popularity during the months of February and September. 

![genres](https://user-images.githubusercontent.com/77643869/115327848-46f9cc00-a155-11eb-935f-9c9f561742b3.png)

Somewhat predictably, Sci-Fi, Adventure, and Animation are some of the most profitable genres, yet it is widely known these are some of the the most expensive competitive categories. However, there are opportunities for Microsoft in other categories that yield above-average profitability, such as Family and Musical movies. 

![actors](https://user-images.githubusercontent.com/77643869/115327930-6d1f6c00-a155-11eb-87e0-536e54930971.gif)

As displayed in the above plot, there are indeed several prominent, "big name" celebrities--also highly rated--that Microsoft, if name recognition is a priority, could opt to hire. Leonardo DiCaprio is the most highly-rated actor in the Top 30 with a performance rating of 5.20 and Robert Downey, Jr. at 3.75. However, there are also actors whom are perhaps not as high-profile, but nevertheless whom rated fairly highly in our model. For example, the actress Idina Menzel was rated a 3.88 on our performance scale (almost as high as Leo, and higher than Robert Downey, Jr.), while having a cost rating of 16, versus DiCaprio's and Downey's ratings of 300+. Lucy Davis' performances were rated as near-comparable at 3.66, and her cost rating of 3 is even more budget-friendly. Daniel Kuluuya's performances were rated higher than both Vin Diesel and Scarlett Johansson, while maintaining one of the lowest cost ratings at 1 (by comparison, Scarlett Johannson and Vin Diesel's cost ratings were both over 100).

## Conclusions 
This analysis leads to three recommendations for Microsoft executives: 
* **Consider timing releases for off-peak months that still show signs of above-average audience turnout,** such as the months of February and September. This will help Microsoft circumvent some of the competition from other studios during the "cluster" months, while also providing opportunities for their products to enjoy above-average popularity. 
* **If startup funding is a significant pain point, consider lower-budget movie genres such as family and musical films,** which tend to earn above-average worldwide gross earnings and are generally known to be cheaper to produce. 
* **Look beyond big-name actors** and engage in recruiting from a pool of lesser-known talent that have the potential to appeal to both mainstream audiences and film critics. 
## Next Steps
The above models utilized the most wide-ranging film-related datasets publicly available, and the results would most likely generalize beyond the data used in this particular dataset. 

These models are reliable because they  reflect widely-accepted trends in the film industry (e.g., films released during the holidays are more popular; adventure films are higher-grossing than documentaries; Leonardo DiCaprio is a highly-rated actor). 

However, these models are also useful for Microsoft because they also uncover windows of opportunity for executives to maximize profit and/or minimize cost--for example, releasing movies in the promising month of February, or hiring lower-profile but high-potential actors. 

As stated in each of the three analysis sections, further analysis could provide opportunities for:
1. More insight into seasonal release trends and their potential impacts on films' popularity;
2. Deeper understanding of the start-up costs and competitition related to each film genre;
3. A wider pool of high-potential actors for Microsoft producers to consider. 
## For More Information 
See the full analysis in the [Jupyter Notebook](./Microsoft_Data_Analysis.ipynb) or review this [presentation](https://github.com/alexiskedo/MicrosoftMovieAnalysis/blob/main/Microsoft_Data_Analysis_Presentation.pdf). 

## Repository Structure

```
├── data
├── Microsoft_Data_Analysis_Presentation.pdf
├── Microsoft_Data_Analysis.ipynb
└── README.md
```
