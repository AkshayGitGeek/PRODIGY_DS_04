# PRODIGY_DS_04
# Traffic Accident Data Analysis

This project provides a comprehensive analysis of traffic accident data using a dataset from Kaggle. It explores patterns related to road conditions, weather, and time of day, and visualizes accident hotspots and contributing factors. The analysis helps identify critical insights and potential areas for intervention.

## Project Structure

The project follows these main steps:

1. **Data Loading**: Importing the accident dataset using `pandas`.
2. **Data Cleaning**: Handling missing values and preparing the data for analysis.
3. **Exploratory Data Analysis (EDA)**:
   - **Time of Day Analysis**: Studying accident frequency across different times of day.
   - **Weather Conditions Analysis**: Analyzing the influence of various weather conditions on accident frequency.
   - **Road Condition Analysis**: Assessing accident frequency by road surface condition.
4. **Hotspot Visualization**:
   - **Geospatial Mapping**: Visualizing accident hotspots on a map using Folium and heatmaps.
5. **Contribution Factor Analysis**:
   - Analyzing correlations among road conditions, weather, time, and accident severity.
6. **Clustering Analysis** (Optional): Using K-means clustering to group accident hotspots for further analysis.

## Requirements

The following libraries are required to run the analysis:

- `pandas`
- `seaborn`
- `matplotlib`
- `plotly`
- `folium`
- `scikit-learn` (optional for clustering)

Install the required libraries via `pip`:
```bash
pip install pandas seaborn matplotlib plotly folium scikit-learn
```

## Code Walkthrough

### Step 1: Import Required Libraries

Import necessary libraries to handle data manipulation, visualization, and geospatial mapping.

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import plotly.express as px
import folium
from folium.plugins import HeatMap
import numpy as np
```

### Step 2: Load the Dataset

Load the dataset from the specified file path:
```python
df = pd.read_csv("path/to/your/dataset.csv")
```

### Step 3: Data Cleaning

Check and handle missing values:
```python
df = df.dropna(subset=['Weather_Condition', 'Road_Condition', 'Time_of_Day', 'Latitude', 'Longitude'])
```

### Step 4: Time of Day Analysis

Analyze and visualize accident frequency by time of day.
```python
# Plotting code here (see project code)
```

### Step 5: Weather Condition Analysis

Visualize accident frequency under different weather conditions.
```python
# Plotting code here (see project code)
```

### Step 6: Road Condition Analysis

Analyze and visualize accident frequency by road condition.
```python
# Plotting code here (see project code)
```

### Step 7: Accident Hotspot Mapping

Create a heatmap to visualize accident hotspots on a map using `folium`:
```python
# Heatmap code here (see project code)
```

### Step 8: Contribution Factor Analysis

Analyze correlations among contributing factors (e.g., severity, weather) using a correlation heatmap.
```python
# Correlation analysis code here (see project code)
```

### Step 9: Clustering of Hotspots (Optional)

Use K-means clustering to identify accident clusters on the map.
```python
# Clustering code here (see project code)
```

## Visualization Outputs

1. **Bar charts** of accident frequency by time of day, weather, and road conditions.
2. **Heatmap** showing accident hotspots based on latitude and longitude.
3. **Correlation matrix** to display relationships among different contributing factors.
4. **Clustered map** (optional) showing grouped accident hotspots for deeper insight.

## Usage

1. Clone this repository and load the dataset.
2. Follow each code block as outlined in the walkthrough.
3. Adjust any dataset column names as needed to match your dataset.

## License

This project is open-source and available under the MIT License.

## Acknowledgments

Dataset provided by [Kaggle](https://www.kaggle.com/), and analysis inspired by common patterns in traffic accident data analytics.
