# Weather-Application-Using-Java
Overview
The WeatherAppProject is a Java-based application that provides weather information, including the current weather and a multi-day forecast. It retrieves data from the OpenWeather API and allows users to view temperature, humidity, wind speed, and weather descriptions. The application features a graphical user interface (GUI) implemented with Swing, allowing for an intuitive and user-friendly experience.

Key Features
Current Weather and Forecast: Fetches real-time weather data and forecasts for a specified number of days.
Unit Preferences: Allows users to switch between metric (°C, m/s) and imperial (°F, mph) units.
Notifications: Provides alerts for high and low temperatures based on user-selected thresholds.
Persistence: Saves user preferences (units and notifications) in a userPreferences.properties file, so they persist across sessions.
Prerequisites
Java JDK: Ensure Java Development Kit (JDK) is installed (version 8 or higher).
Gson Library: The gson-2.11.0.jar file should be in the lib directory.
Setup and Execution
Step 1: Compile the Code
To compile the code, open a terminal or command prompt, navigate to the project directory (WeatherAppProject), and run the following command based on your operating system.

On Windows
javac -cp "lib\gson-2.11.0.jar" -d bin src\*.java
On Linux/macOS
javac -cp "lib/gson-2.11.0.jar" -d bin src/*.java
This command compiles all .java files in the src folder and places the generated .class files in the bin folder.

Step 2: Run the Application
After compilation, you can run the WeatherSwingApp class from the bin directory, which serves as the entry point.

On Windows
java -cp "bin;lib\gson-2.11.0.jar" WeatherSwingApp
On Linux/macOS
java -cp "bin:lib/gson-2.11.0.jar" WeatherSwingApp
This command launches the application with a graphical interface.

Usage
Current Weather: Use the GUI to enter the city name and view current weather details.
Weather Forecast: Specify the city and number of days for forecast data through the interface.
Preferences: Update unit preferences (metric or imperial) and enable/disable notifications for high/low temperature alerts via the settings menu.
Notes
The userPreferences.properties file in the resources folder saves the user’s preferences for units and notifications.
Ensure to set your API key in the WeatherAPIManager class if you replace the code or API credentials.
