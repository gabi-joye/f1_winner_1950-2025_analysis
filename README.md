


<img width="173" height="198" alt="Screenshot 2025-11-04 185328" src="https://github.com/user-attachments/assets/27a23295-f4e1-4df5-a343-60c342464470" />
<img width="238" height="160" alt="Screenshot 2025-11-04 185353" src="https://github.com/user-attachments/assets/f20578f9-b5d2-4375-ae9e-739a160efd70" />

These images show the top 5 teams and racers that have won the most races in the Grand Prix.

<img width="572" height="445" alt="Screenshot 2025-11-04 185436" src="https://github.com/user-attachments/assets/9f0bc58e-f4b7-4aa4-9d9f-27a0917fd639" />



<img width="590" height="443" alt="Screenshot 2025-11-04 185422" src="https://github.com/user-attachments/assets/a6e872f0-f7c1-4b16-8407-0ad5809b7f9e" />



<img width="593" height="446" alt="Screenshot 2025-11-04 185511" src="https://github.com/user-attachments/assets/98bb1649-4aa4-434c-ac3a-8347ade67128" />



<img width="558" height="451" alt="Screenshot 2025-11-04 185457" src="https://github.com/user-attachments/assets/9a744f22-9b3e-4bc3-b812-499292873649" />

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
🧹 Data Cleaning
No missing or null values were found
Converted:
date → datetime
time → timedelta (numeric format)
Identified outliers in race time, which were considered during analysis

⚠️ Note: This dataset does not account for technological advancements in cars over time, which likely impacts race performance trends.

🎯 Key Questions
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
