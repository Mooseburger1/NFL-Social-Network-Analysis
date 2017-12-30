# NFL-Social-Network-Analysis
Performing Social Network Analysis on the 2017 NFL schedule - Scraping the web with Python and Pandas
This was a project performed to find out just how the NFL generates their schedule for all 32 two teams. Using Python, Pandas, and Networkx, a social network analysis is performed by scraping the schedule for all 32 teams from espn.com. 

Networkx was used to graph the nodes and edges, and ultimately export a .gml file, which is included in the repository. This .gml file is then imported into an open source program called Gephi in order to create the "publish quality" image contained in both the Jupyter notebook and the .png file in the repository. 

For Clarification:
An extra step was needed in parsing the data for 2 teams, The Dallas Cowboys and the Arizona Cardinals. Both of these teams had an extra preseason game (the Hall of Fame game) which altered the structure of their website being scraped as compared to the other 30 teams. This extra step is the first step performed in the code (notebook)
