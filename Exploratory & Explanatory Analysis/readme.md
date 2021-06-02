# Bay Wheels Data Exploration
## by Laila Madany


## Dataset

The data consisted information about individual approximately 1,860,000 trips made in a bike-sharing system covering the greater San Francisco Bay area in 2018. The attributes included start time, trip duration, user type as well as additional measurements such as gender and birth date. The dataset can be found in their repository [here](https://s3.amazonaws.com/fordgobike-data/index.html).

The raw data was assessed and some of its quality issues were cleaned. Erroneous datatypes were converted into their corresponding appropriate ones and missing birth year and gender data were removed. In addition, 5 features were engineered for further insights and more interesting findings! When assessing the engineered age feature, there were some outliers which needed further verification so those were removed.


## Summary of Findings

In 2018, there was a high demand usually around 8-9 AM and then 5-6PM. People used Bay Wheels more on weekdays (Monday to Friday) than weekends. Regarding monthly trends, January had the lowest number of trips and the trend was usually higher in early-mid autumn and summer months. The majority of trips fell into short rides with durations between 5 to 10 minutes. Also, the trip distribution included some outliers with the longest trip lasting 1438 minutes. We will exclude the 1% extreme outliers from visualizations when necessary as it will distort them.

There were much more males than females but on average females have slightly longer trips. Most users were subscribers rather than customers. There were no specific patterns related to each gender but during the first 3 months in 2018, we observed a really small male to female ratio for customers. However, starting April, the number of trips of male customers drastically increased. The average age is around 35 years old and people aged between 30-40 years old had the highest number of trips during the first 5 months in 2018. Afterwards, those aged 18-20 started taking the leading position up until the end of the year.

Each user type have different patterns and exhibit different preferences. Subscribers depict the behavior of school/work commuters where they used the service mostly during weekdays with the number of trips reaching its peak at 8AM & 5 PM. Their overall hourly/daily peak was Tuesday 8 AM and the peak month has been October. On the other hand, customers are more casual and flexible, having higher number of trips during weekends. Their overall hourly/daily peaks were Saturday 2 PM & Friday 5 PM and the peak month has been July. Lastly, the average trip duration for customers is longer than subscribers. Subscribers have a relatively unchanging trip durations. For Customers, their average trip duration drastically jumps on Saturday. In general for both user types, trips are shorter during weekdays and longer during weekends.


## Key Insights for Presentation

For the presentation, the focus was on how the user type affected the time-related features which highlighted the different behaviors and patterns of Bay Wheels users. The average trip duration and the most trips taken in terms of time of day, day of the week, or month of the year depended on whether the user is a Customer or Subscriber. I started by introducing the User types depicting their relative frequencies through a pie chart and absolute frequencies through a countplot (also used as an element for repetition). We followed by their average weekly trip duration, then using a heatmap to combine the time of day and day of the week showing the user type trends.

Afterwards, the monthly trend line of the user type was plotted. Finally as a bonus (extra) graph, we've included the monthly trend line across our 4 age groups due to the interesting pattern there. I've renamed the legend age groups for a cleaner visual. All graphs were also polished by adding titles, formatting ticks and renaming axes as well as legend titles.

## Resources

https://www.freecodecamp.org/news/how-to-combine-multiple-csv-files-with-8-lines-of-code-265183e0854/
https://stackoverflow.com/questions/43427564/display-all-informations-with-data-info-in-python
https://www.w3resource.com/pandas/dataframe/dataframe-dropna.php
https://knowledge.udacity.com/questions/179434
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.dt.hour.html
https://matplotlib.org/3.1.1/gallery/pie_and_polar_charts/pie_features.html
https://matplotlib.org/3.1.0/gallery/color/named_colors.html
https://stackoverflow.com/questions/7082345/how-to-set-the-labels-size-on-a-pie-chart-in-python
https://www.journaldev.com/39342/seaborn-line-plot
https://jamesrledoux.com/code/group-by-aggregate-pandas
https://dfrieds.com/data-analysis/bin-values-python-pandas.html
https://kanoki.org/2020/04/20/how-to-create-bins-in-pandas-using-cut-and-qcut/
http://seaborn.pydata.org/tutorial/categorical.html?highlight=bar%20plot
http://seaborn.pydata.org/generated/seaborn.catplot.html#seaborn.catplot
https://riptutorial.com/pandas/example/6874/aggregating-by-size-versus-by-count
https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.title.html
https://stackoverflow.com/questions/6541123/improve-subplot-size-spacing-with-many-subplots-in-matplotlib
https://stackoverflow.com/questions/33446029/how-to-change-a-figures-size-in-python-seaborn-package
https://stackoverflow.com/questions/44954123/rotate-xtick-labels-in-seaborn-boxplot
https://matplotlib.org/3.1.1/api/font_manager_api.html
https://stackoverflow.com/questions/12750355/python-matplotlib-figure-title-overlaps-axes-label-when-using-twiny

