# Python-projects-re

## Visualizing Recent Earthquakes using a free dataset from the USGS website.
1. Import libraries: We import pathlib for handling file paths, 
    JSON for parsing the GeoJSON data, and plotly.graph_objects for creating the visualization.
2. Load GeoJSON data: We use pathlib.Path to create a path object for the GeoJSON file and then open it  and load
    the contents into a Python dictionary using JSON.loads().
    Extract data: We extract the latitude, longitude, and magnitude values from the GeoJSON data and store them in separate lists.
4. Create the map: We create a go.Scattergeo object using Plotly, specifying the latitude, longitude, and magnitude values.
    We set the marker size and color based on the magnitude, using the Viridis color scale and adding a colorbar
    to indicate the magnitude range.
    We update the layout of the figure to set the title, scope, and appearance of the map.
5. Finally, we use fig.show() to display the map.
    This code will create an interactive map showing the locations of recent earthquakes, with marker size and color
    representing the magnitude. You can customize the map further by adjusting the color scale, adding more details, or
    using different types of markers.

##### NB: the negative mag values were changed to positives using the abs function   
