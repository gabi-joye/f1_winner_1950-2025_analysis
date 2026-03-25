# Formula 1 Grand Prix Winners Analysis (1950–2025)

Exploring performance trends, race times, and winning dominance in F1 history

# Project Overview

This project analyzes a historical dataset of Formula 1 Grand Prix winners from 1950 to 2025. The goal is to uncover trends in race performance, identify dominant teams and drivers, and explore how race times have evolved over decades.

# Dataset

The dataset contains 1,142 rows and 9 columns, including:

Column	Description
date	Race date
continent	Location by continent
grand_prix	Name of the race
winner	Winning driver
team	Winning constructor
time	Total race time
laps	Number of laps
year	Year of race

# Data Cleaning
No missing or null values were found
Converted:
date → datetime
time → timedelta (numeric format)
Identified outliers in race time, which were considered during analysis

Note: This dataset does not account for technological advancements in cars over time, which likely impacts race performance trends.

# Key Questions
Which team has the most Grand Prix wins?
Which driver has the most wins?
How have average race times changed over decades?
Are there outliers in race times?
Do certain circuits produce faster race times?
What are the fastest and slowest winning times in history?

# Key Insights

Top Teams & Drivers
Identified the top 5 teams and drivers with the most wins in F1 history
Highlights long-term dominance patterns in the sport

Race Time Distribution
Race times show a right-skewed distribution
Indicates most races cluster around faster times
20 outliers detected in race duration

Race Time Trends Over Time
Average race times decrease over decades
Suggests improvements in:
Car performance
Track conditions
Racing strategies

# Adjusted Analysis: Lap Time

To account for varying race lengths, average lap time was analyzed:

Downward trend still persists
Confirms that faster race times are not just due to fewer laps

Note: The 2020s decade includes partial data

# Correlation: Laps vs Race Time

Found a moderate positive correlation (0.476)
More laps generally lead to longer race times, as expected

# Key Takeaways

Certain teams and drivers dominate historically
Race performance has improved significantly over time
Even after adjusting for laps, races are getting faster
Outliers exist and should be considered in deeper statistical analysis
External factors (technology, regulations) likely play a major role

# Skills Demonstrated

Data cleaning and preprocessing
Data type transformation (string → datetime/timedelta)
Exploratory Data Analysis (EDA)
Data visualization and interpretation
Correlation analysis
Analytical storytelling

# Future Improvements

Include car specifications or regulation eras
Analyze circuit-specific performance trends
Build predictive models for race outcomes or times
Add interactive dashboards (Tableau / Power BI)





# https://www.kaggle.com/datasets/julianbloise/winners-formula-1-1950-to-2025
