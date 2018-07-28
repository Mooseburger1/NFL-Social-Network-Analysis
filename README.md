# NFL-Social-Network-Analysis
Performing Social Network Analysis on the 2017 NFL schedule - Scraping the web with Python and Pandas
This was a project performed to find out just how the NFL generates their schedule for all 32 two teams. Using Python, Pandas, and Networkx, a social network analysis is performed by scraping the schedule for all 32 teams from espn.com. 

Networkx was used to graph the nodes and edges, and ultimately export a .gml file, which is included in the repository. This .gml file is then imported into an open source program called Gephi in order to create the "publish quality" image contained in both the Jupyter notebook and the .png file in the repository. 

For Clarification:
An extra step was needed in parsing the data for 2 teams, The Dallas Cowboys and the Arizona Cardinals. Both of these teams had an extra preseason game (the Hall of Fame game) which altered the structure of their website being scraped as compared to the other 30 teams. This extra step is the first step performed in the code (notebook)



![NFL SOCIAL NETOWRK OUTPUT](https://github.com/Mooseburger1/NFL-Social-Network-Analysis/blob/master/NFL%20Schedule.png)

# Analysis Results
-----------------------------
Analysis: The NFL is made up of two conferences - the NFC and the AFC. Each conference has 16 teams and those 16 teams are broken up into 4 seperate divisions:

AFC NORTH NFC NORTH AFC SOUTH NFC SOUTH AFC EAST NFC EAST AFC WEST NFC WEST

Running the Social Network Analysis with Networkx and Gephi, I used the "Forced Atlas 2" algorithm inside of gephi to cluster the teams as seen above. The clusters correctly depict the 4 teams that make up a division. That is why there are 4 nodes in each cluster. The algorithm also places the clusters in the middle of the other clusters a particular cluster plays the most.

For example:

The divisions are displayed in the image as follows: Starting at the top of the graph and going clockwise ORANGE - AFC WEST PURPLE - NFC EAST PURPLE2 - NFC WEST BLUE - AFC SOUTH BLUE2 - AFC NORTH GREEN - NFC NORTH GREEN2 - NFC SOUTH ORANGE2 - AFC EAST

So as you can see, the AFC West plays each other twice a year and thats how they got clustered together, and then the bulk of their schedules consist of playing teams from the NFC EAST and the AFC EAST, and thats why AFC WEST cluster was placed between these two clusters. The same logic applies to all other clusters
