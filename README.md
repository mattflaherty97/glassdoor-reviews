# A Glassdoor Analysis

Firm-level shocks can affect employee satisfaction in positive or negative ways. In this work, I scrape reviews from glassdoor.com and analyze shocks to find the effects of these shocks on employee satisfaction. I am able to find shocks using term frequency and by using information about COVID such as work from home orders.

# Data

The data includes ratings, information about the employee such as whether the employee currently works at the company or not, employee title, date of review, three approval categories (recommend company, CEO approval, company outlook). The data also include free-text responses such as pros, cons, and advice to management.

Ratings range from 1-5 and employees can leave sub-ratings in six categories. The approval categories contain a check mark for approval, an X for disaproval, a line for neutral, or a circle for NA.

# Repo Structure

Using the repository, the user should be able to run code that will scrape reviews from [glassdoor.com](https://www.glassdoor.com/member/home/index.htm). Unfortunately, Glassdoor only allows users to scrape data if they have 1) created and account and 2) left a review. Without the completion of these steps, you will not be able to scrape any data.

1.  To collect the data, the user must run the Glassdoor scrape using [glassdoor_scrape.ipynb](https://github.com/mattflaherty97/glassdoor-reviews/blob/main/glassdoor_scrape.ipynb)
2.  Following the scrape, the user must clean the data with [clean_scrape_data.ipynb](https://github.com/mattflaherty97/glassdoor-reviews/blob/main/clean_scrape_data.ipynb)
3.  After the data is clean, sentiment scores can be calculated using a couple approaches in the [glassdoor_sentiment_analysis.ipynb](https://github.com/mattflaherty97/glassdoor-reviews/blob/main/glassdoor_sentiment_analysis.ipynb) file
4.  With clean data and sentiment scores, the [analysis.ipynb](https://github.com/mattflaherty97/glassdoor-reviews/blob/main/analysis.ipynb) file can be used to gather the results

# Necessary packages

* [selenium](https://selenium-python.readthedocs.io/)
* [pandas](https://pandas.pydata.org/)
* [numpy](https://numpy.org/)
* [time](https://docs.python.org/3/library/time.html)
* [warnings](https://docs.python.org/3/library/warnings.html)
* [statistics](https://docs.python.org/3/library/statistics.html)
* [nltk](https://www.nltk.org/)
* [re](https://docs.python.org/3/library/re.html)
* [seaborn](https://seaborn.pydata.org/)
* [matplotlib](https://matplotlib.org/)
* [sklearn](https://scikit-learn.org/stable/)
