# DATA200---Final-Project
### Introduction
When professional baseball teams are putting together their opening day 26-man roster, they have many decisions to make. One of their hardest decision is to decide between rostering a reliable veteran or a high-upside young player. The veteran will normally give you consistent numbers while the young player could waste a roster spot or breakout to become a star player after. MLB teams are turning to the data in order to make this difficult decision. 

In this study we will be using the advanced metric **wOBA (Weighted On-Base Average)** to predict if a player will have a breakout season. wOBA measures a player's overall offensive contribution per plate apperance by assigning a weight for each type of hitting event.

$$wOBA = \frac{0.690 \times uBB + 0.722 \times HBP + 0.888 \times 1B + 1.271 \times 2B + 1.616 \times 3B + 2.101 \times HR}{AB + BB - IBB + SF + HBP}$$

wOBA takes into account the outcome of each plate appearance and its significance, making it a more reliable metric compared to simpler stats such as hitting average or on-base percentage

### Goals
1. Predict a player's wOBA in the following season
2. Predict weather a player will have a breakout season

we will validate our models using the 2024 season and test our model with the 2025 season

### Data Description
We have two data sets that we are going to be pulling raw data from, **Batting.csv** and **People.csv**. **Batting.csv** has yearly raw batting stats per player along with the team, the data involves raw batting stats like player ID, **AB**(At bats), **1B**(Singles), **2B**(Doubles), **3B**(Triples), **HR**(Home Runs), **BB**(Walks), **SF**(Sacrifice Fly) and much more. **People.csv** takes the player ID from **Batting.csv** and links it to a real players name, weight, height, birth information and more. Merging these two data sets together we get a data set which includes players names, weight, height and all raw batting stats. This merged data set will be very useful when creating variables and plots as it contains all data needed for the study.   
