# Optimal-Bus-Route-Finder
Bus route search engine based on a graph constructed from processed GTFS data and using a modified Dijkstra's algorithm.

# Route Finder

## Overview
This project aims to create a route-finding system for public transportation in Gdańsk. It utilizes a 2 km x 2 km grid overlaid on the city map, where each grid cell is uniquely identified. The system processes bus stop data, assigns trips to the grid, and optimizes route selection based on available data.

The Jupyter Notebook guides users through:
1. Generating a geospatial grid overlay on the Gdańsk map.
2. Importing and processing public transportation data, including bus stops and schedules.
3. Assigning trips to grid cells and visualizing the network.
4. Implementing a modified multi-source Dijkstra’s algorithm to determine the shortest routes\.
5. Exporting the computed shortest path as an interactive HTML map.

## Features
- Generates a grid-based map of Gdańsk.
- Processes public transportation data, including bus stops and arrivals.
- Assigns bus trips to grid cells for efficient route calculation.
- Implements shortest path algorithms for optimized route suggestions.
- Allows data updates when needed to prevent graph overload, rather than updating daily\.
- Generates an interactive HTML map of the shortest path.

## Installation
1. Clone the repository:
   ```sh
   git clone <repository_url>
   cd route-finder
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```sh
   jupyter notebook "Route Finder.ipynb"
   ```

## Usage
- Open the Jupyter Notebook and execute the cells step by step to process the data.
- Modify the input dataset to analyze different timeframes or locations.
- The computed shortest path is saved as `shortest_path.html` and can be opened in any web browser for visualization.
- Below is a sample visualization of the shortest path:

 <img src="shortest_path.png" alt="Shortest Path" width="500"/>
 
## Dependencies
The project requires the following Python libraries:
- pandas
- geopandas
- numpy
- folium
- matplotlib
- networkx

Ensure that all dependencies are installed before running the notebook.

## Data
The dataset includes:
- Bus stops and their locations.
- Bus trip data from November 7th.
- The system allows for data updates when necessary to prevent graph overload.

## Future Improvements
- Implementing real-time data integration.
- Enhancing route optimization algorithms.
- Expanding coverage beyond Gdańsk.

## License
This project is licensed under the MIT License.

## Author
Developed by [Your Name]. Contributions are welcome!




