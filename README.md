# 115_Personal_Dataset_Project
The reposition contain the files and code for my personal data set project. 

# Motivation
I really enjoy watching football and some of the biggest controversies on Sundays can come from penalties. 

# Data Process
The source of all this penalty data comes from a repository here on GitHub called “nflfastR”. This “nflfastR” is a set of functions that has been efficiently
scraping play-by-play data from the NFL since 1999. There is a ton of data including first downs, yards per play, etc. but I only selected the data on penalties. All I did to process the data was make sure there is no duplicate data and add two more columns. The first column I added was a net amount between penalties at home and penalties away for each team. The second column I added was a "More Away" column with boolean value that depends net amount calculated in the previous column. If the net amount in the first added column is positive, then the value in the second added column is false for not having more penalties in away games than home. If the value is the first added column is negative, then the boolean value in the second added column would be true for having more away flags than home ones.

# Visualizations
## Figure 1

<img src="https://raw.githubusercontent.com/isiverWSU/115_Personal_DataSet_Project/main/Figure1-HomeVersusAway.png">
Caption: Each team in the figure above lies on the scatter plot in relation to how many penatlies they received at home games and how many they received while away.
This data is based on penalties received during the 2020 NFL Regular Season. 

## Figure 2

<img src="https://raw.githubusercontent.com/isiverWSU/115_Personal_DataSet_Project/main/Figure%202%20-%20HomeVersusAway2.png">
Caption: Here is the same scatter plot from Figure 1 but clustered by teams who have more penalties at home or away. 

##Figure 3

<img src="https://raw.githubusercontent.com/isiverWSU/115_Personal_DataSet_Project/main/Figure3-NetPenaltiesBarChart.png">
Caption: This is a bar chart representing each teams net amount of flags. The positive bars represent teams that had more penalties at home games while the negative bars indicate teams that had more penalties at away games. I added a color key to make it more distinguishable. 

# Analysis 

I did some very simple exploratory data analysis to come to the conlusion that ~2/3 of NFL Teams are penalized more often while being the away team. I did this by plotting the Home column against the Away column and then clustered them according to the Net Amount between the two. Right off the bat in Figure 2 you can see that more teams seem to fit under the area where having more away penalties is true. This is just a rough clustering estimate however so I wanted to take it one step further. In Figure 3 you will see that I plotted the Net Penalties column in a bar chart showing positive and negative values. Here we can see that only 11 teams have a positive amount of net flags, meaning they had  more flags thrown against them at Home than Away. 11/32 teams is roughly 34% so the other ~66% of teams indeed are penalized more as the away team.
