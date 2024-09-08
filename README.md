# SustainAI
<img src="https://github.com/samer07/SustainAI/blob/main/logo.png" alt="Logo" width="250"/>
# Welcome to SustainAI


## Key Features

### Data Collection 

We have utilized a dataset from **Rosetta** that provides detailed information on renewable energy assets and projects across various regions in Australia. The dataset includes:

- Asset type
- Site name
- Technology type
- Fuel type
- Geographical coordinates (latitude and longitude)
- Associated organizations

### Dataset Source:
[Rosetta Renewable Energy Dataset - July 2024 (Points)](https://renewables.networkmap.energy/Network%20Map%20Renewables%20July%202024%20(Points).csv)

---

## Weather Information Integration

We have augmented the renewable energy dataset with weather data for specific geographical locations (based on latitude and longitude). This allows us to factor in critical environmental variables that impact the efficiency of solar power generation, including **temperature** and **solar irradiance**.

### Weather Data Sources:
- **Solar Irradiance Data** from [NASA POWER](https://power.larc.nasa.gov/)
- **Temperature Data** from [Open Meteo](https://open-meteo.com/)

By combining these data sources, we can account for essential environmental factors such as temperature fluctuations, solar irradiance, and other weather conditions, enabling more accurate predictions for solar power generation efficiency.

---

## Purpose of the Project

The integration of weather data with the renewable energy assets dataset allows for:
- **Enhanced Energy Forecasting**: Accurate predictions of energy output based on environmental factors like solar irradiance and temperature.
- **Improved Site Selection**: Factoring in weather patterns, such as long-term solar irradiance trends, to determine optimal locations for new solar projects.
- **Proactive Maintenance**: Monitoring environmental conditions that could impact the efficiency of solar panels, enabling predictive maintenance strategies.
- **Visualization and Analysis**: Clear graphical representations of energy production potential, taking into account environmental conditions for different geographical locations in Australia.

---

## How to Access the Dataset

1. **Rosetta Renewable Energy Dataset**:
   - Download the dataset from [here](https://renewables.networkmap.energy/Network%20Map%20Renewables%20July%202024%20(Points).csv).

2. **NASA POWER**:
   - Access the solar irradiance data through [NASA POWER API](https://power.larc.nasa.gov/).
   
3. **Open Meteo**:
   - Get real-time and historical temperature data from [Open Meteo API](https://open-meteo.com/).
   - 
## Visualization 
Solar Power Plant Analysis
Geographical Distribution
<img src="https://github.com/samer07/SustainAI/blob/main/Geographical%20Distribution%20of%20Solar%20Power%20Plants.jpg" alt="Geographical Distribution of Solar Power Plants" width="600"/>
This map shows the geographical distribution of solar power plants across different regions.

Multivariate Analysis
<img src="https://github.com/samer07/SustainAI/blob/main/Multivariate%20Analysis%20of%20Capacity%2C%20Latitude%2C%20and%20Longitude.jpg" alt="Multivariate Analysis of Capacity, Latitude, and Longitude" width="600"/>
This chart presents a multivariate analysis of solar power plant capacity in relation to latitude and longitude.

Capacity Distribution
<img src="https://github.com/samer07/SustainAI/blob/main/capacity.jpg" alt="Capacity Distribution" width="600"/>
This graph illustrates the distribution of solar power plant capacities.

Technology Impact
<img src="https://github.com/samer07/SustainAI/blob/main/technology%20imapct%20on%20location%20and%20capacity.jpg" alt="Technology Impact on Location and Capacity" width="600"/>
This visualization demonstrates the impact of technology on the location and capacity of solar power plants.


## Prediction and Clustering

We predict solar potential using the **RandomForestRegressor** model with the following features:

- **Latitude**
- **Longitude**
- **Temperature**
- **Wind Speed**
- **Cloud Cover**
- **Humidity**

## Clustering of Power Plants

Clustering is performed based on power plant location and weather conditions to group similar regions. 

![Clustering of Power Plants](https://github.com/samer07/SustainAI/blob/main/clustering.jpg)





