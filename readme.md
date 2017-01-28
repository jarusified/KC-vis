## Running 
To run the visualisation, we need to create a server to render the data files. (Or) visit https://eidos1406.github.io/


A simple python server would work good. 

'''

python -m SimpleHTTPServer 8888

'''

## Implementation 

* D3js is the toolkit which was used for visualisation of the Kansas city crime rate for the year 2014. A timeline is a chart that depicts how a set of resources are used over time. 

* The x-axis of the graph is a moving timeline starting from Jan 1st, 2014 to Dec 31st, 2015. 

* The y-axis of the graph denotes the crime rate on a particular date, ranges from 1 (lesser crime) - 10 (High level crimes).

* Circles are used to denote the number of crimes on a specific day. The average number of crimes in a day is 270 crimes/day. 

* The dataset used is [Kansas city crime alert](https://data.kcmo.org/Crime/crime-data/9u7z-x596). The dataset is sorted by date and report number from the timeline Jan - 2014 to Dec - 2014. 

* The Offence codes are mapped based on the level of crime to values 1-10 manually. The offence codes are stored in an array of objects and are used to place the circles based on the crime level. 

* The circles have an animation while they enter. The animation shrinks the size from 70px to a size represented by the Crime count. 

* Colors, Pink and red are used to represent the gender of people who perform the crime. Pink is used to represent the circles when female crimes are in domination and red, otherwise. 

## Inferences

* This visualisation gives a clear idea on the rate of crimes performed on each day. We can use this data to find which month has the maximum number of crimes. 

* In general, the circle sizes are smaller as they tend to higher crime level, showing that only smaller offences take part in the city of kansas.
