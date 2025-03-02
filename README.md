# belly-button-challenge
Overview
This project is an interactive data visualization dashboard for exploring microbiome data collected from human belly buttons. It provides insights into the bacterial cultures found in different test subjects using dynamic bar and bubble charts.

Technologies Used
HTML, CSS, Bootstrap: For structuring and styling the web interface.
JavaScript (D3.js, Plotly.js): For fetching and visualizing data.
JSON Data Source: Hosted remotely to provide sample metadata and bacterial cultures.
Features
Dropdown Menu: Users can select a test subject ID to update the charts and metadata panel dynamically.
Demographic Information Panel: Displays subject-specific metadata.
Bar Chart: Shows the top 10 bacterial species found in a sample.
Bubble Chart: Displays the distribution of bacteria cultures per sample.
File Structure
index.html
This file defines the web interface:

A title and description of the dashboard.
A dropdown (#selDataset) that allows users to select a test subject ID.
A demographic information panel (#sample-metadata).
Containers for bar and bubble charts (#bar and #bubble).
Links to external libraries: Bootstrap (for styling), D3.js (for data manipulation), and Plotly.js (for chart rendering).
Loads app.js to handle interactivity.
app.js
This script is responsible for:

Fetching microbiome sample data from an external JSON source.
buildMetadata(sample): Updates the demographic information panel with details of the selected test subject.
buildCharts(sample): Creates a bar chart (top 10 bacterial species) and a bubble chart (bacterial culture distribution).
init(): Runs on page load, populating the dropdown and displaying the first sample’s data.
optionChanged(newSample): Updates charts and metadata when a different test subject is selected.
How It Works
The dashboard loads and fetches the dataset from the external JSON source.
A dropdown menu is populated with available sample IDs.
Selecting an ID updates:
The demographic info panel.
The bar chart (Top 10 bacteria in the sample).
The bubble chart (Bacteria distribution).
Users can explore different samples interactively.
Setup Instructions
Open index.html in a browser.
Ensure an internet connection to load external data and libraries.
Interact with the dropdown to explore microbiome data.
