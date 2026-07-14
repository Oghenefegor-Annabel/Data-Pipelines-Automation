# Data-Pipelines-Automation
Built a simple ETL pipeline using real-time weather data using API
# Project Overview
This project demonstrates an end-to-end ETL (Extract, Transform, Load) workflow using real-time weather data obtained from the OpenWeather API. The objective was to retrieve current weather information for multiple cities, clean and structure the data using Python and Pandas, and perform basic exploratory analysis to compare weather conditions across the selected locations.

The project showcases practical skills in API integration, data extraction, data transformation, data cleaning, and basic data analysis.

# Data Source
Source: Openweather API
API Endpoint: https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric
Data Type: JSON
Cities Used: Lagos, Benin, Port Harcourt, Warri, Abuja, Ibadan,Zaria,Enugu,Onitsha,Jos

# ETL Process
EXTRACTION: The data was retrieved from Openweather API  using requests library in python, the API response was retrieved in JSON format. The fields City Name, Humidity, Weather Condition, Temperature, Date and Time, Wind Speed.

TRANSFORMATION:
* Converted JSON data into a dataframe.
* Renaming columns for readability.
* Converting date and time values to datetime format.
* Ensuring numeric fields had the correct data types.
* Standardizing weather descriptions.

LOAD:
The cleaned dataset was saved as clean_weather_data.csv, making it ready for analysis.

# Tools Used
* Jupyter Notebook : Development environment
* Python: Programming language
* OpenWeather API: Data source
* Pandas : Data transformation and analysis
* Requests : API connection and retrieval

# STEPS TAKEN
1. Installed the required libraries (requests and pandas).
2. Connected to the OpenWeather API using a personal API key.
3. Retrieved weather data for Lagos, Abuja, and Port Harcourt.
4. Extracted relevant weather fields from the JSON response.
5. Stored the extracted records in a Python list.
6. Converted the list into a Pandas DataFrame.
7. Renamed columns and corrected data types.
8. Validated the dataset for missing or inconsistent values.
9. Saved both raw and cleaned datasets as CSV files.
10. Performed basic comparative analysis on temperature, humidity, and weather conditions.

# KEY FINDINGS
1. The coolest city in the list of cities is Enugu.
2. The hottest city in the list of cities extracted is Warri.
3. The average temperature is 25°C
4. Weather conditions varied across the selected cities, showing differences in local atmospheric conditions.
5. The analysis demonstrated how real-time API data can be transformed into a structured dataset suitable for business or environmental analysis.
