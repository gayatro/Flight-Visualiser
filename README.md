# Visualise Bird Flight
https://gayatro.github.io/Flight-Visualiser/
# Flight Visualizer Instructions

## Overview

The Flight Visualizer is a web-based tool that visualizes flight data in a 3D environment using CesiumJS and a 2D map using Leaflet. The tool allows you to visualize a flight path based on data from a CSV file containing geographical coordinates.

## Prerequisites

Before using the Flight Visualizer, you need to have the following:
- A valid [Cesium Ion Access Token](https://ion.cesium.com/signin/tokens?page=1). You can create a free account and generate a token if you don’t have one.
- A CSV file containing the flight data. The CSV file must contain the following columns: `Longitude`, `Latitude`, `Altitude`, and `Bearing` (case sensitive).

## Setting Up the Data

1. Ensure your CSV file is properly formatted with the required columns: `Longitude`, `Latitude`, `Altitude`, and `Bearing`.
2. If necessary, visit the [GitHub repository](https://github.com/gayatro/fly-visual/tree/main) to run the "data-processor" script, which calculates the required parameters and formats your data for this simulator.

## How to Use

1. **Open the Application**: Launch the HTML file containing the Flight Visualizer in your web browser.

2. **Input Cesium Ion Access Token**:
   - Enter your Cesium Ion Access Token in the provided input box.

3. **Initialize the Map**:
   - Click the `Initialise Map` button. This will load the CesiumJS viewer and the Leaflet map.

4. **Upload Your CSV File**:
   - Click the `Choose File` button and upload your CSV file. The program will process the file and prepare the data for visualization.

5. **Start the Visualization**:
   - After uploading the CSV file, click the `Play` button to start the flight visualization.
   - Use the slider labeled `Flight Progress` to manually control the flight progress.
   - Adjust the viewing direction with the `Viewing Direction` slider and change the camera pitch using the `Pitch` slider.

6. **Pause or Resume the Visualization**:
   - You can pause the flight at any time by clicking the `Pause` button. Click it again to resume.

## Additional Controls

- **Altitude Display**: The current altitude of the flight is shown at the top-right corner of the screen.
- **Map View**: The 2D map on the bottom-right corner shows the flight path and the current position.

## Important Notes

- The visualization will automatically loop back to the start once it reaches the end of the flight path.
- Ensure your CSV data is correctly formatted. The program will alert you if the required columns are missing or if no valid data is found.

## Troubleshooting

If the visualization does not start:
- Verify that your Cesium Ion Access Token is valid and entered correctly.
- Ensure that your CSV file contains valid numerical data for all required columns.
- Check the console in your browser's developer tools for any error messages.

## Enjoy the Simulation!

Explore and analyze your flight data in a dynamic 3D environment combined with a 2D map view.
