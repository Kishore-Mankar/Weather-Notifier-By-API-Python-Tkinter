# Weather Notifier By API🌦️

A simple weather application built with Python and Tkinter that lets users check current weather conditions for a city. It retrieves weather data from the OpenWeatherMap API and displays the results in a graphical window.

## Features

- Search for current weather by city name.
- Display the city and country.
- Show current temperature in Celsius.
- Show the “feels like” temperature.
- Display minimum and maximum temperatures.
- Show humidity and wind speed.
- Display a weather icon and general weather condition.
- Validate empty city-name input and show an error if a city cannot be found.
- Show a connection error if a request to the weather service fails.

## Requirements

- Python 3
- An internet connection
- An OpenWeatherMap API key
- Python packages:
  - `requests`
  - `Pillow`

The GUI uses Python's built-in `tkinter` library.

## Installation

1. **Install Python 3** if it is not already installed.

2. **Download or clone this project** and open a terminal in the project folder.

3. **Install the required packages:**

   ```bash
   pip install requests pillow
   ```

4. **Configure your OpenWeatherMap API key.**

   The script uses an API key in the `api_key` variable. For security, use your own key and avoid committing API keys to a public repository. You can load it from an environment variable instead.

   For example, replace the hard-coded key with:

   ```python
   import os

   api_key = os.getenv("OPENWEATHERMAP_API_KEY")
   ```

   Then set the `OPENWEATHERMAP_API_KEY` environment variable to your key before running the application.

## Run the Application

Run the Python file from your terminal:

```bash
python "Weather GUI.py"
```

A window titled **Weather Conditions** will open.

1. Enter a city name.
2. Click **Submit**.
3. View the current weather information in the results window.

## Weather Information Displayed

| Field | Description |
|---|---|
| City and country | Location returned by the weather API |
| Temperature | Current temperature in °C |
| Feels like | Apparent temperature in °C |
| Weather condition | General condition, such as Clouds or Rain |
| Minimum / maximum temperature | API-reported minimum and maximum temperatures in °C |
| Humidity | Relative humidity in percent |
| Wind speed | Wind speed in metres per second |
| Weather icon | Icon provided by OpenWeatherMap |

## API and Network Notes

- Weather data is retrieved from the OpenWeatherMap Current Weather API.
- An internet connection is required.
- API usage limits apply. The original script comments advise staying below 60 runs per minute; check your account's current OpenWeatherMap plan and limits.
- If the city is not found, the application displays an error message.
- If a network request fails, the application displays a connection error.

## Project Structure

```text
Weather-GUI/
├── Weather GUI.py
└── README.md
```

## Troubleshooting

- **`ModuleNotFoundError` for `requests` or `PIL`:** Run `pip install requests pillow`.
- **The application cannot connect:** Check your internet connection and try again.
- **A city is not found:** Check the spelling and try the city name again.
- **API errors:** Verify that your OpenWeatherMap API key is valid and that your account has access to the endpoint.
- **Tkinter is unavailable:** Install the Tkinter package appropriate for your operating system or Python distribution.

## Technologies Used

- Python
- Tkinter
- Requests
- Pillow (PIL)
- OpenWeatherMap API

## Author

Mankar Kishore Babu 
B.Tech-Information Technology


## License

This Project is open source and available for learning and educational purposes
