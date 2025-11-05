The dataset we will be using today is a cobination of all F1 Grand Prix winner from 1950-2025. The columns include the date the race took place, the continent, the Grand Prix, the winner name, the team, the time, the laps and the year.

has 1142 rows and 9 columns. There are no blank or N/A values, there are however a few ouliers in the time columns. 
While analysing this data we will also need to take into account that race cars have had mechanical advancements that are not noted in this dataset.

Questions going into our analysis:
What team has had the most racers win the Grand Prix?
What racer has won the most Grand Prix races?
What is the average winning race time per decade?
Are there any outlires in our race time category?
Do different circuits have better average winning race times than other?
What is the fastest time ever to win a Grand Prix?
What is the slowest time ever to win a Grand Prix?

The first thing I did was clean my data, there are no null values that needed attended, so I moved on to datatypes.
When I first looked at my column datatimes the time and date columns where strings so I had to change them into numaric datatypes to be able to work with them in the way I wanted.
For the time column I created a new column with a timedelta datatype, i then turned my  date column from a string to a datetime datatype.



. This will give us the average winning race time per decade. *Note that the decade 2020 only includes 5 years rather than 10. I than create a lineplot to help us visualize this data().

Next I want to find out if there are any outliers in our time_delta column. To do this i first have to find the z-scores for my times. I subtract the time_delta from the Time_deltas mean then devide that by the standard deviation of the time_delta column assigning this to a new column called time_z-score. An outlier is any z-score that is less than -3 or grater than 3 so I create a column that will print True if it is




# https://www.kaggle.com/datasets/julianbloise/winners-formula-1-1950-to-2025
