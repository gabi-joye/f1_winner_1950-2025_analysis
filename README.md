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
When I first looked at my column datatimes the time and date columns where strings so I had to change them into numaric datatypes to be able to work with thm in the way I wanted.
To change the time column I first had to use .replace to update the sytax of a few datapoints. After the sytax was the same throughout the column I used pd.to_timedelta to  create a new
column that I would be able to aggregate with. I then turned my attention to the date column and ust pd.to_datetime to turn my column into a datetime datatype.

Once my data was clean I started to preform my analysis. Firstly I used a .groupby method to find the team and racer with the most wins.

# https://www.kaggle.com/datasets/julianbloise/winners-formula-1-1950-to-2025
