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
For the time column I created a new column with a timedelta datatype, I then turned my  date column from a string to a datetime datatype.

<img width="173" height="198" alt="Screenshot 2025-11-04 185328" src="https://github.com/user-attachments/assets/27a23295-f4e1-4df5-a343-60c342464470" />
<img width="238" height="160" alt="Screenshot 2025-11-04 185353" src="https://github.com/user-attachments/assets/f20578f9-b5d2-4375-ae9e-739a160efd70" />

These images show the top 5 teams and racers that have won the most races in the Grand Prix.

<img width="572" height="445" alt="Screenshot 2025-11-04 185436" src="https://github.com/user-attachments/assets/9f0bc58e-f4b7-4aa4-9d9f-27a0917fd639" />

This hystogram of the distrobution of winning race times shows a right skew. This means that most of the data shows a faster race time. There are also 20 outlires found in the time_delta column used for this graph whitch may contribute to the skew.

<img width="590" height="443" alt="Screenshot 2025-11-04 185422" src="https://github.com/user-attachments/assets/a6e872f0-f7c1-4b16-8407-0ad5809b7f9e" />

This line plot shows the average winning race times in our dataset. After see ing this I decided to look for reasons there might be such variation between the race times. When doing this i realized that different races have differen t amount of laps so I made a new lineplot showing average lap time rather than the race as a whole. That line plot is shown below. 
*Note 2020 only has 5 years of data rather than 10.

<img width="593" height="446" alt="Screenshot 2025-11-04 185511" src="https://github.com/user-attachments/assets/98bb1649-4aa4-434c-ac3a-8347ade67128" />

The drop in race time is still very porominate in our second graph whitch may be due to facters not noted in this dataset such as machanical advacments in race cars between 1950 and 2025.

After seeing the changes between my 2 line plots I created a scaterplot to visualize the correlation between race time and laps and found a moderate positive correlation(0.475797) between the to.

<img width="558" height="451" alt="Screenshot 2025-11-04 185457" src="https://github.com/user-attachments/assets/9a744f22-9b3e-4bc3-b812-499292873649" />







# https://www.kaggle.com/datasets/julianbloise/winners-formula-1-1950-to-2025
