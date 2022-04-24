# Celebrities and Divorce
We seek to build a model that does predictive analysis on whether a celebrity will divorce. This particular model had an accuracy of 82% after testing multiple statistical algorithms, cross validations, and hyperparameter tuning. Ultimately, CatBoost was the best performing algorithm.

I found interest in building this particular model after seeing the whole Will Smith and Chris Rock fiasco at the Oscars 2022. It got me thinking about the divorce rate among celebrities as opposed to the average American. We've seen Kim Kardashian and Kanye West's messy break and I started to think if it was possible to build a model that could possibly predict where a celebrity's relationship would last by looking at 10,000 other celebrities. 

There are certainly many outside factors that affect a decision that's hard for me to quantify and factor into this model but I wanted to see if I could find some accuracy with a basic model that looked at age, sex, number of spouses, marital status, the amount of kids and such. Ideally, I would also find a way to quantify how successful each actor/actress would be and information about their spouses, but for the sake of keeping this simpler, I'm stickign to the features that I have. 

I built a web scraper that looked at the first 10,000 celebriteies in IMDB's ranking based off of their 'StarMeter.' I'm not familiar with how that ranking occurs but I'm guessing it has to do with the amount of searches every few days or so. 

Anyways, I pull the names and the URL of the first 10,000 names and from each URL, I pull the birthdate, deathdate (if available), spouse info, children. I also pull sex of the celebrity by running a counter of gender pronouns in the biography of each celebrity, so it may not be the most accurate but is the best I could think of without running it on another website.

In this repository, I will be importing various jupyter notebooks for data scraping, exploratory data analysis, and running statistical algorithms.


# How to Setup
The IMDB file allows you to scrape 10,000 celebrities off of IMDB's website. Using functions to pull specific information, I was able to clean the data into a dataset ready for EDA and analysis testing. 

The IMDB_EDA file explores and breaksdown the demographic of the sample size of 10,000 celebrities. I use Seaborn and Matplotlib to create graphs to visualize the data. I then use several different supervised learning algorithms to compare which performs the best. 
