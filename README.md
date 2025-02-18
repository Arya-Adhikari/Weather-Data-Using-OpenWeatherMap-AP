Weather Data Collection Script

Overview

This Python script fetches real-time weather data for a list of predefined cities using the OpenWeatherMap API. The data is collected every 5 seconds for a duration of 1 minute and is then stored in a JSON file.

Features

Fetches current weather data for multiple cities

Extracts temperature, weather conditions, humidity, and wind speed

Collects data at regular intervals for a set duration

Saves the collected data into a JSON file

Prerequisites

Ensure you have Python installed along with the required dependencies:

pip install requests pandas

Setup

Obtain an API key from OpenWeatherMap.

Replace the api_key variable in the script with your actual API key.

Usage

Run the script using:

python weather_script.py

Output

The script collects weather data for the specified cities every 5 seconds for a total duration of 1 minute.

Data is stored in weather_data.json in JSON format.

Sample JSON output:

{"city": "New York", "temperature": 15.5, "weather": "clear sky", "humidity": 78, "wind_speed": 5.1, "timestamp": "2025-02-17 12:30:00"}

Notes

The script currently runs for 1 minute (originally set for 15 minutes, but changed for quick testing). You can modify the loop duration by adjusting while (time.time() - start_time) < 60:.

The time interval between requests for each city is set to 5 seconds to prevent exceeding API limits.

License

This script is provided under the MIT License.
