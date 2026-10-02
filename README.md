#  Simple Weather App - Flask

A simple weather web application built with **Python and Flask** that allows users to search for the current weather of a location by entering its **city, state, and country**.

The application uses the **OpenWeather API** to find the location coordinates and retrieve current weather information.

##  Features

*  Search weather by city, state, and country
*  Display current temperature in Celsius
*  Display current weather condition
*  Display weather description
*  Display weather icon information
*  Uses OpenWeather Geocoding API to find location coordinates
*  API key is loaded from environment variables
*  Simple Flask web interface

##  Technologies Used

* **Python**
* **Flask**
* **Requests**
* **python-dotenv**
* **HTML / Jinja2**
* **OpenWeather API**

##  Project Structure

```text
Simple-Weatherapp-Flask/
│
├── templates/
│   └── index.html
│
├── app.py
├── weather.py
├── requirement.txt
├── .gitignore
└── README.md
```

> The virtual environment and `.env` file are kept locally and should not be uploaded to GitHub.

##  How It Works

1. The user enters a **city, state, and country** in the web application.
2. Flask receives the submitted information.
3. The application sends the location to the OpenWeather Geocoding API.
4. The latitude and longitude of the location are retrieved.
5. The application uses those coordinates to request current weather data.
6. The weather information is returned and displayed on the webpage.

##  Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yash-gupta-py/Simple-Weatherapp-Flask.git
```

### 2. Go into the project directory

```bash
cd Simple-Weatherapp-Flask
```

### 3. Create a virtual environment

Windows:

```bash
python -m venv weather
```

### 4. Activate the virtual environment

PowerShell:

```powershell
.\weather\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirement.txt
```

### 6. Create a `.env` file

Create a `.env` file in the project root:

```env
WEATHER_API_KEY=your_openweather_api_key
```

Do **not** upload your `.env` file to GitHub.

### 7. Run the application

```bash
python app.py
```

The application will normally be available at:

```text
http://127.0.0.1:5000
```

##  Environment Variables

This project uses `python-dotenv` to load the OpenWeather API key from a `.env` file.

Required variable:

```env
WEATHER_API_KEY=your_api_key_here
```

The `.env` file should be included in `.gitignore` so that your API key is not committed to the repository.

##  Example

Enter a location such as:

```text
City: Toronto
State: ON
Country: Canada
```

The application uses the location information to find its coordinates and then retrieves the current weather.

##  What I Learned

This project was built to practice:

* Python programming
* Flask web development
* Working with APIs
* Sending HTTP requests with `requests`
* Using environment variables
* Working with `.env` files
* Using Git and GitHub
* Creating a basic web application with Flask

##  Future Improvements

Possible improvements for the project:

* Add a 5-day weather forecast
* Add better error handling for invalid locations
* Add loading indicators
* Improve the user interface
* Add responsive design for mobile devices
* Display humidity, wind speed, and other weather details
* Add weather history
* Deploy the application online

##  Author

**Yash Gupta**

GitHub: [@yash-gupta-py](https://github.com/yash-gupta-py)
