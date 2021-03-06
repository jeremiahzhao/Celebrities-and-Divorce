# Celebrities and Divorce
I seek to build a model that does predictive analysis on whether a celebrity will divorce. This particular model had an accuracy of 82% after testing multiple statistical algorithms, cross validations, and hyperparameter tuning. Ultimately, CatBoost was the best performing algorithm.

![image](https://user-images.githubusercontent.com/98020536/164996702-16401f30-e746-4e3a-ac3b-ba5d3721ca3a.png)

I found interest in building this particular model after seeing the whole Will Smith and Chris Rock fiasco at the Oscars 2022. It got me thinking about the divorce rate among celebrities as opposed to the average American. We've seen Kim Kardashian and Kanye West's messy break and I started to think if it was possible to build a model that could possibly predict where a celebrity's relationship would last by looking at 10,000 other celebrities. 

There are certainly many outside factors that affect a decision that's hard for me to quantify and factor into this model but I wanted to see if I could find some accuracy with a basic model that looked at age, sex, number of spouses, marital status, the amount of kids and such. Ideally, I would also find a way to quantify how successful each actor/actress would be and information about their spouses, but for the sake of keeping this simpler, I'm stickign to the features that I have. 

I built a web scraper that looked at the first 10,000 celebriteies in IMDB's ranking based off of their 'StarMeter.' I'm not familiar with how that ranking occurs but I'm guessing it has to do with the amount of searches every few days or so. 

![Screen Shot 2022-04-24 at 2 11 46 PM](https://user-images.githubusercontent.com/98020536/164996746-3175bbc8-b555-44e8-b614-c6ef755a225f.png)

Anyways, I pull the names and the URL of the first 10,000 names and from each URL, I pull the birthdate, deathdate (if available), spouse info, children. I also pull sex of the celebrity by running a counter of gender pronouns in the biography of each celebrity, so it may not be the most accurate but is the best I could think of without running it on another website.

In this repository, I will be importing various jupyter notebooks for data scraping, exploratory data analysis, and running statistical algorithms.


# How to Setup
The IMDB file allows you to scrape 10,000 celebrities off of IMDB's website. Using functions to pull specific information, I was able to clean the data into a dataset ready for EDA and analysis testing. 

The IMDB_EDA file explores and breaksdown the demographic of the sample size of 10,000 celebrities. I use Seaborn and Matplotlib to create graphs to visualize the data. I then use several different supervised learning algorithms to compare which performs the best. 

# EDA
These are the following plots I was able to create to reflect more of the demographics of the celebrities pulled.
![Celeb1](https://user-images.githubusercontent.com/98020536/164996883-71492513-8fe8-489f-8d36-43bdecb58b93.png)
![celeb2](https://user-images.githubusercontent.com/98020536/164996923-3be26f5d-2f8e-4908-bd4f-8c1e19c243c9.png)
![celeb3](https://user-images.githubusercontent.com/98020536/164996928-beb676ca-afb1-4094-b5d5-d569e7485fcf.png)
![celeb4](https://user-images.githubusercontent.com/98020536/164996929-b0a250c7-04d9-4593-a817-b055de684a6e.png)





