# Investigating the Flight Data In 2007 from the Bureau of Transportation Statistics

## by Chidiebere Chukwuemeka


## Dataset
> The dataset under consideration is from the Bureau of Transportation Statistics. The dataset contains information on time performance of flights. The dataset is for consideration will only cover the year 2007 and can be downloaded directly from their website. The description is posted on their website in detail

link to dataset: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7

> The 2007 Flight dataset contains 7453215 entries and 29 columns(representing features in the dataset). The features of interest will be the Month, Distance, TaxiIn,TaxiOut, CarrierDelay, WeatherDelay, SecurityDelay, LateAircraftDelay, AirTime, ArrDelay, DepDelay, Cancellation. We can use this to get insights that are neccessary for the research.

- First step taken during the Data Exploration was to import the data, view the data in other to understand the features of the data set

- Second step was the data cleaning phase and wrangling.

- Third step was to start asking questions and making well informed plots resulting from the type of the data and the question asked. The charts started with the univariate plots werein when neccessary transfomations were made.

- Next was the Bivariate and Multivariate chart where multiple variables and features of interest were explored to seek answers to the questions raised.

- The plots comprises of charts from `Matplotlib` and `Seaborn` libraries as the plots consist of `Barplots`, `scatterplot`, `pairplot`, `histogram` etc.


## Summary of Findings

In the exploration phase, i found that their were more Cancellation made because of `Carrier(s)` followed by cancellation by `Weather`, `National Air System` and `Security` respectively. I also found that their seem to be a very close range between the top three months with most flights(Aug, Jul and Mar). Also the August holiday period seem to have the highest flights made during the year 2007 as people will tend to spend the long holiday relaxing in diferent locations. Its also noticable that December was amongst the buttom four as I myself was expecting higher travels during that period in the calender.

Their was a strong correlation for Departure and Arrival Delay when fights are not cancelled. The study also found that the relationship between the `Distance` and `Airtime` of flights were seen to be near perfect. There were also noticable positive corellation between `Arival` and `Depature` delay. `Late Air Craft Delay` also had a positive correlation with `Arival` and `Depature` delay.

The study also shows that their was a weak (if not even negative) relationship between Monthy flights, Distance covered and the reasons for flight Cancellation.


## Key Insights for Presentation

The key take away for this presentation is that monthly delays caused by `weather` and `late air craft` have a greater overall impact than delays caused by other factors. This was achieved by querying the data to make sure all delays were above 0 mins, then merged the resulting delay variables. The searborn lineplot was helpful to a great deal as it clearly showed the mean plots of each delay variables across each month. 