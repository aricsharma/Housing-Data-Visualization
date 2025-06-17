# Housing Data Visualization

This project creates an interactive map to visualize housing data from the California Housing Dataset using Python. Each data point is represented by a circle marker scaled by the average number of rooms and color-coded by median house value. The resulting map is saved as an HTML file, making it easy to explore and share insights visually.

## 🗺️ Features

- Interactive map centered on California
- Circle markers positioned using latitude and longitude
- Marker **color** indicates median house value (from green to red)
- Marker **size** reflects the average number of rooms
- Popups display detailed housing stats: median value, rooms, population, income
- Built-in MiniMap plugin for orientation and navigation
- Generates a standalone `real_estate.html` file

## 🛠️ Tech Stack

- **Language**: Python  
- **Libraries**:  
  - `pandas` – data handling  
  - `matplotlib` – color mapping  
  - `folium` – interactive maps  
  - `scikit-learn` – built-in housing dataset (`fetch_california_housing`)  
  - `folium.plugins` – MiniMap support  

## 📈 Dataset

The dataset used is the **California Housing Dataset**, which includes:
- `Latitude` and `Longitude` of neighborhoods
- `MedHouseVal`: Median house value
- `AveRooms`: Average number of rooms
- `Population` and `MedInc`: Socioeconomic context

Fetched using:
```python
from sklearn.datasets import fetch_california_housing
