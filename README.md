# 115_Personal_Dataset_Project
The reposition contain the files and code for my personal data set project. 

# Motivation
I really enjoy watching football and some of the biggest controversies on Sundays can come from penalties. 

# Data Process
The source of all this penalty data comes from a program called “nflfastR”. This “nflfastR” is a set of functions that efficiently
scrapes play-by-play data from the NFL. There is a ton of play-by-play data including first downs, yards per play, etc. but I only selected the data on penalties. All I did to process the data was make sure there is no duplicate data and add two more columns. The first column I added was a net amount between penalties at home and penalties away for each team. The second column I added was a "More Away" column with boolean value that depends net amount calculated in the previous column. If the net amount in the first added column is positive, then the value in the second added column is false for not having more penalties in away games than home. If the value is the first added column is negative, then the boolean value in the second added column would be true for having more away flags than home ones.

# Visualizations
## Figure 1

<img src="https://raw.githubusercontent.com/isiverWSU/115_Personal_DataSet_Project/main/Figure1-HomeVersusAway.png">
Caption: Each team in the figure above lies on the scatter plot in relation to how many penatlies they received at home games and how many they received while away.
This data is based on penalties received during the 2020 NFL Regular Season. 

## Figure 2

# Analysis 
