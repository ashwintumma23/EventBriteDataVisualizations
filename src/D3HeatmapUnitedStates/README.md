Through this data visualization, we see the distribution of events state-wise for United States. Eventbrite's data is accessible through their JSON API. This visualization makes use of the same API to query and get the data related to the region (state) (filtered by country="US"). 

### Features
This section enlists the features of the D3 heatmap data visualization. 
* Displays the data for the all the regions of the United States.
* Upon hovering the mouse over each state, a detailed view of the state, along with the number of events occuring/ occured in the state is displayed as a tooltip (See screenshots below).
* The darker the color of the state, more the number of events that were held in that state and vice versa.

### Files
This section provides a brief description of the all the files and their purpose in this directory. 
* `DataPoints.txt`: File containing the count of the number of events that have occured/ will occur in each state.
* `GetStatesCounters.py`: Python script for fetching the "region" data from the Event Brite JSON API and counting the number of occurences for events in each state of the United States. (See file header  comments for detailed description and elaborate comments).
* `PopulateJSON.py`: Python script for reading the data from the data points text file and populating the JSON file with the required data and its required format.
* `README.md`: This file
* `D3HeatMapDisplay.html`: HTML5 code for rendering the Javascript heatmap in the browser
* `jquery.tipsy.js`: Javascript for displaying the tooltips
* `tipsy.css`: CSS file for the tooltip rendering
* `us.json`: File which is generated by the `PopulateJSON.py` script using `us.json.template` which is fed as the input to the `D3HeatMapDisplay.html` for rendering purposes.
* `us.json.template`: Template for the JSON file.
* `usheatmap.js`: Main Javascript file which contains all the co-ordinates for all the states in the United States.

### Code References
* DataMaps - Open Source code for creating maps [website](http://datamaps.github.io/).  
* Tipsy [Website](http://bl.ocks.org/ilyabo/1373263) - For displaying tips on mouse hover

### Screenshots 
Following figure shows the screenshot of distributions of events based on their count in the United States. The state being hovered upon in this screenshot is New York. 
 ![My image](https://github.com/ashwintumma23/EventbriteDataVisualizations/blob/master/Images/D3Maps.png)
 
 Following figure shows the screenshot of distributions of events based on their count in the United States. The state being hovered upon in this screenshot is California. 
 ![My image](https://github.com/ashwintumma23/EventbriteDataVisualizations/blob/master/Images/D3California.png)
 
### Other Enhancements: 
 This section lists some of the enhancements that are possible for in this data visualization. 
 * Aggregation of all the code in the same python script file can be done easily
 * Different colors can be used for rendering the maps. An example of which is shown in the screenshot below.
![My image](https://github.com/ashwintumma23/EventbriteDataVisualizations/blob/master/Images/RedD3Map.png)