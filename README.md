Intro to project

When I first approached the Citibike data website, I was impressed with the amount of data that had been collected and was available. After my initial impression, I subsequently became overwhelmed by where to start my analysis! Quickly, I decided to look at the data over time. In order to do this, I needed to carefully select my time periods and develop a strategy for paring back the emmense data available. I ended up chosing the years between 2018 and 2020 to evaluate. Because of the data structure (files split by month, by year), I wanted to save myself a little time by selecting data from the first month of each quarter of the three years (January - Q1, April - Q2, July - Q3, and October - Q4). This decision left me with 12 CSV's to download.

Next, I needed to pare the data within the files. I wrote an .ipnyb file in Jupyter Notebook that read the CSV files into 12 dataframes, created a new column converting trip duration to minutes instead of seconds, cleaned data and removed outliers, took a random sample of 500,000 trips from each file, and joined them into a final CSV.

"Phenomena" 1

In my first dashboard, I took a look into User Type. From January 2018 to January 2020, the proportion of Single-Use Riders (aka "Customers" in the dataset) and Subscribers was relatively steady, about 95% subscribers to about 5% single-use riders on average. At the end of Q2 in 2020, the global COVID-19 pandemic hit. I believe this was the cause of the subsequent shift in the User Type proportions. Between April 2020 and October 2020, single-use riders increased as a proportion of ridership by about 10%, to an average of 16% of ridership.

After reviewing the shift in ridership makeup, I wanted to evaluate how those two groups differ in they way they use the bikes from year-to-year. What I found was that generally, since 2018, single-use riders have used the bikes for "Very Long" rides (rides lasting longer than 15 minutes on average, likely joyrides or sight-seeing) while subscribers have tended to take "Short" trips (between 5 and 10 minutes, likely commuting in the city). In 2020, while single-use riders did not dramatically change their trip duration, subscribers increased their "Very Long" trips by more than 10%. The scatter plot shows the dark blue (2020) has increased in both trip duration and trip distance for both groups, meaning riders are using Citibikes more for recreating than in 2018 and 2019.

With all of the chaos and uncertainty in the world right now, at least in New York City, it seems people are finding a little more entertainment in a nice bike ride around the city. If Citibike can convert the influx of single-use customers into subscribers, and continue to promote bike riding as a healthy, safe way to recreate during a pandemic, there may be some goodwill and positive brand benefit to be gained.

"Phenomena" 2

