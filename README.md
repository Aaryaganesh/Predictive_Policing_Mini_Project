
# Crime Data Analysis and Visualization

This project involves the analysis and visualization of crime data to derive insights and generate heatmaps for better understanding of crime patterns. Using Python libraries such as `pandas` and `folium`, the dataset is cleaned, processed, and visualized through heatmaps and clustered markers.

## Table of Contents
- [Dataset](#dataset)
- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Outputs](#outputs)

## Dataset
Link to Dataset : https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/about_data
The project utilizes a CSV dataset (`Crime_Data_from_2020_to_Present_20241125.csv`) containing crime records with fields such as:
- **Crime Code and Description** (`Crm Cd Desc`)
- **Victim Details** (Sex, Descent)
- **Location Details** (Latitude, Longitude, Area Name)
- **Premise Details** (Code, Description)
- **Date of Occurrence**

## Features
1. **Data Cleaning**:
   - Columns with excessive missing values are removed.
   - Missing values in relevant columns are filled with default or placeholder values.
   - Rows with missing critical information are dropped.
   
2. **Data Analysis**:
   - Frequency of crime types.
   - Most common crime types in specific areas (e.g., Central).
   - Unique crime types and their occurrences.

3. **Data Sorting**:
   - Crime dataset sorted by crime type and frequency for better readability.

4. **Visualizations**:
   - **Heatmaps**:
     - Heatmap for all crime locations.
     - Heatmap for specific crimes (e.g., "Vehicle - Stolen").
   - **Clustered Markers**:
     - Crime locations displayed with popups showing details like date, location, and crime description.
   - **Top Crime Hotspots**:
     - Heatmaps for the top 5 most frequent crime types with a legend.

## Requirements
- Python 3.x
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `folium`
  - `folium.plugins` (for `HeatMap` and `MarkerCluster`)

## Setup
1. Clone this repository or download the code files.
2. Install the required Python libraries:
   ```bash
   pip install pandas numpy folium
   ```
3. Place the dataset file `Crime_Data_from_2020_to_Present_20241125.csv` in the project directory.

## Usage
1. Run the main script to clean and analyze the data:
   ```bash
   python main_script.py
   ```
2. View the generated heatmaps and marker maps:
   - `crime_heatmap.html`
   - `vehicle_stolen_heatmap.html`
   - `top_5_crime_hotspots_with_legend.html`
3. Open the `.html` files in a browser to interact with the maps.

## Outputs
1. **Data Cleaning**:
   - Cleaned dataset saved as `Sorted_Crime_Dataset.csv`.
   - Dataset sorted by crime frequency saved as `Crime_Dataset_Sorted_By_Frequency.csv`.

2. **Visualizations**:
   - Heatmaps for overall crimes, specific crime types, and hotspots.
   - Clustered markers for easy identification of high-crime areas.

3. **Insights**:
   - Frequency of crime types.
   - Identification of most frequent crime types and areas with high crime rates.
  


**Crime Data Visualization and Analysis Using QGIS**

---

### **Description**
This project visualizes and analyzes crime data using QGIS. The geospatial data is plotted on an interactive map to identify crime hotspots and trends. Key features include point plotting, heatmap generation, and clustering for effective visualization.

---

### **Features**
1. **Point Mapping**:
   - Each crime incident is represented as a point on the map using latitude (`LAT`) and longitude (`LON`).
   - Crime types are categorized and visualized with unique colors.

2. **Heatmap Analysis**:
   - A heatmap layer is created to highlight areas with high crime density.
   - Kernel density estimation is used to visualize crime intensity.

3. **Clustering**:
   - Crime locations are grouped into clusters to identify patterns and hotspots.

4. **Basemap Integration**:
   - Basemaps (e.g., OpenStreetMap) provide geographic context for crime data.

5. **Categorical Visualization**:
   - Crime types are styled distinctly based on `Crm Cd Desc`.

---

### **Data Source**
- The dataset contains crime data with attributes such as latitude, longitude, and crime type.

---

### **Workflow**
1. **Data Preparation**:
   - Input data in CSV format with `LAT` and `LON` columns.
   - Ensure CRS is set to **WGS 84 (EPSG:4326)**.

2. **Visualization**:
   - Load data into QGIS.
   - Apply symbology for point mapping and categorical styling.

3. **Analysis**:
   - Generate heatmaps and clusters to identify high-crime areas.

4. **Export**:
   - Final map layouts are exported as PNG or PDF.

---

### **Dependencies**
- **QGIS** (version X.X or higher)
- **QuickMapServices Plugin** (for basemaps)

---

### **Usage**
1. Open the QGIS project file or load the provided CSV data.
2. Customize visualization settings as needed.
3. Generate heatmaps or clusters for advanced analysis.
4. Export the map for reporting or presentation.

---

### **Output**
- A QGIS-generated map showing:
  - Individual crime locations.
  - High-crime areas via heatmaps.
  - Clustered crime patterns.
![Screenshot 2024-12-09 162318](https://github.com/user-attachments/assets/177ac864-86cf-4bdf-a88c-e459616bef35)

