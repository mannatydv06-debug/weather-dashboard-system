Weather Dashboard (Requests Version)

A command-line weather dashboard that searches for a city and displays current weather using the free Open-Meteo geocoding and forecast APIs. Open-Meteo does not require an API key for this example.

Features :-
Modular WeatherAPIClient class
City-name lookup using geocoding
Current temperature, feels-like temperature, humidity, wind speed, precipitation, and conditions
Human-readable weather descriptions
Request timeouts and friendly messages for network failures
Handles blank and unknown city names
Uses a configurable request timeout

Requirements :-
Python 3.9 or newer recommended
requests package

Setup :-
Install Python.
Open a terminal in this project folder.
Install the dependency:
python -m pip install -r requirements.txt
Run:
python main.py
Enter a city name, for example Delhi or Tokyo.

API and Credentials :-
This version uses:
Open-Meteo Geocoding API: https://geocoding-api.open-meteo.com/v1/search
Open-Meteo Forecast API: https://api.open-meteo.com/v1/forecast
No API key or .env file is required. Do not add secret credentials to GitHub. The app requires an internet connection to fetch live data.

Example Output :-
Exact values depend on the live weather response.
CodeNova Weather Dashboard (Open-Meteo; no API key required)
Enter a city name: Delhi

========== WEATHER DASHBOARD ==========
City: Delhi
Conditions: Mainly clear
Temperature: <live value> °C
Feels like: <live value> °C
Humidity: <live value> %
Wind speed: <live value> km/h
Precipitation: <live value> mm
=======================================
The condition and numeric values above are illustrative placeholders, not a live forecast.

Error Testing :-
Enter a made-up city name to test the location-not-found message.
Disable internet briefly to test the connection error.
Use a slow or unavailable connection to test timeout handling.

Project Files :-
main.py — application and API client
requirements.txt — external dependency list
README.md — setup, API, and testing instructions

Limitations :-
This is a command-line application, not a graphical dashboard. Weather values depend on Open-Meteo availability and its response. HTTP status errors and malformed responses are handled with friendly messages.

Learning Outcomes :-
Practise API integration, JSON parsing, classes, exception handling, HTTP requests, and formatting data for users.