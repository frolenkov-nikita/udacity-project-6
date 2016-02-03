Project 6, Data Visualization
-----------

1. Goals
==========

The goal is to create explanatory visualization of the provided dataset.

2. Dataset
=========

The data set contains 1,157 baseball players with following fields:

- handedness (right-,left- or both-handed)
- height (in inches)
- weight (in pounds)
- batting average
- home runs

Visualization should show how baseball player are performing depending on their handedness, height and weight.


3. Sketch and ideas
========

Initial ideas were concentrated in the sketch https://dl.dropboxusercontent.com/u/1274349/sketch-66502801.png

Goals are:

 1) to keep accent on players performance (HR and BA) rather than on their physical parameters (weight, height, handedness)
 2) to keep information on one, readable, plot
 3) to have easy player's performance comparison by weight, height and handedness
 4) to show dependency between player's performance and physical parameters
 5) to center on a specific finding in the data
 6) to allow reader to explore the data

 As I have only one plot and I need to show difference between groups I need to go with bar chart which
is best for comparison between different groups. Scatter plot or line graph may work if I use few plots but on one plot they will make
a lot of noise: many lines/dots overlapping each other.

I need to show how 2 continuous (HR & BA) values depend from physical parameters on one plot, therefore there is no way I can display HR & BA on orthogonal axes, therefore two Y axes are required. X axis will be for the categorical parameter handedness which will group bars. Color differentiation between HR & BA bars will be used. Another option is to have second Y axis “mirrored”, I will use it if readers have complains about color differentiation. Bars are located vertically, as I want to have X values be located intuitively, from left to right: “left-handed”, “right-handed”, “both-handed”. 

The possibility to see the influence of weight & height is hardly desired but there is no chance to somehow add this information on the plot and keep it readable,
therefore weight & height should be somehow displayed outside of the plot. 
Making them adjustable by a slider allows reader to explore the data.

Two clickable links “Players with top HR” and “Players with top AVG” will show the reader a specific finding about which players have best performance.

4. Feedback
========

I've received some feedback from udacity's forum and google plus group:

"Very nice visualization! I like how interactive it is, and especially the buttons for height and weight. The only thing that was hard for me to grasp was what the shades of the colors of the bars represent.

An interesting thing that I've noticed was that the players with the highest weight (230-240) are left handed and have very high HR and AVG. Overall it appears that left-handed players have better performance." by KaterinaB

"Hello Nikita,

the most pronounced relationship that I noticed is that left-handed players achieved more homeruns than right-handed and both-handed players; that relationship seems to be more pronounced for players with low weight (160-180) than for players with weights above 180.

One question I had, when playing around with the selectors, was how large the group of players is that I had chosen. So I would find it helpful to get displayed the number of players currently selected in total, or how many players are represented by each bar. That would allow to get a sense of how meaningful the bars are.

What confused me a little is that at some points of the selectors (e.g., weight=180) the bars seem to flip. At other points, the bars corresponding to both-handed players jump to the left and overlap those corresponding to left-handed players.

All in all, I find this a clear visualization that allows to easily search for relationships within subgroups of players." by david_308760

"Very advanced technically graph, congratulations. Here are the answers of the questions:

Do you have any questions about the dataset? No

My interpretation of the chart:
- presented comparison of the number of home runs and batting average by Handedness;
- option to explore the influence of the weight and the height of the players over their performance.

Were you able to notice any relationships?
- Left-handed players have higher HR
- Tall low weight left handed players have very high HR :)

Is there something unclear or hard to understand in this visualization?
- I can't understand this transition (swapping) of the columns. In addition it prevents me to trace the change of the size.
- It is not clear what information is coded by the colour saturation
- Are we speaking about average home runs? Not clear from the title.

It would be useful to see somehow the number of players in the selected Weight-Height group.﻿" by Krasin 


5. Improvements after feedback
=========

I decided to:

- Improve legend
- Fix transition
- Add height & width measure units
- Improve plot title
- Display how many players are there with selected width & height
