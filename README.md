Belly Button Biodiversity Dashboard
This repository contains a data visualization project that analyzes microbial biodiversity using sample data. The project dynamically displays charts and metadata based on user-selected sample IDs. It leverages D3.js for data fetching and Plotly.js for rendering visualizations.

Features
Interactive Dropdown Menu: Allows users to select a sample ID and view the corresponding data dynamically.
Metadata Panel: Displays demographic and sample-specific metadata for the selected sample.
Bubble Chart: Visualizes the relationship between OTU IDs and sample values with markers sized by sample abundance.
Bar Chart: Displays the top 10 OTUs for each sample in a horizontal bar chart.
Dynamic Updates: Automatically updates the visualizations and metadata panel when a new sample is selected.

JavaScript Functions
init()
Initializes the dashboard:
Fetches samples.json.
Populates the dropdown menu with sample IDs.
Displays the metadata and charts for the first sample.
buildMetadata(sample)
Fetches and displays metadata for the given sample ID.
Updates the panel with ID #sample-metadata.
buildCharts(sample)
Fetches and visualizes data for the given sample ID.
Renders:
Bubble Chart: Shows OTU IDs vs. sample values with tooltips.
Bar Chart: Displays the top 10 OTUs for the sample.
optionChanged(newSample)
Triggered when a new sample is selected from the dropdown menu.
Updates charts and metadata for the selected sample.

Technologies Used
D3.js: For fetching and manipulating JSON data.
Plotly.js: For creating interactive charts.
HTML/CSS/JavaScript: For the dashboard's structure and interactivity.