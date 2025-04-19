# API-INTEGRATION-AND-DATA-VISUALIZATION

*COMPANY*:CODTECH IT SOLUTIONS

*NAME*:R.Rajasri

*INTERN ID*:CT04DA237

*DOMAIN*:PYTHON PROGRAMMING

*DURATION*:4 WEEKS

*MENTOR*:NEELA SANTHOSH

#This project demonstrates how to integrate a public API with Python and visualize the fetched data using powerful Python libraries. Specifically, it connects to the OpenWeatherMap API to retrieve weather forecast data and visualizes temperature trends over time using Matplotlib and Seaborn.

Tools and Libraries Used
Python
Python is a high-level, general-purpose programming language that is widely used for scripting, automation, data science, and web development. It’s known for its simplicity and readability, making it ideal for beginners and professionals alike.

requests
The requests library is a standard tool in Python for making HTTP requests to web APIs. In this project, it is used to send a request to the OpenWeatherMap API and receive the weather forecast data in JSON format. This data contains various weather-related attributes such as temperature, humidity, weather description, and timestamps.

json (implicitly used via .json() method)
The API response comes in JSON format, which is a lightweight data-interchange format. Python’s built-in JSON tools allow easy parsing and extraction of necessary values from the response.

matplotlib.pyplot
Matplotlib is a widely-used 2D plotting library in Python. The pyplot module is used to plot data and customize visualizations. In this script, it creates a line chart that maps temperature against time to show how the weather evolves.

seaborn
Built on top of Matplotlib, Seaborn provides a high-level interface for attractive and informative statistical graphics. It makes charts look visually appealing with minimal code. Here, it’s used to enhance the line plot of temperature trends with a clean and modern look.

datetime
This built-in module helps manipulate date and time in Python. It is used to convert the timestamp from the API (dt_txt) into Python datetime objects for proper plotting on the x-axis.

Project Workflow
The script sends a request to the OpenWeatherMap API using the user’s city and API key.

The API returns forecast data for the next 5 days in 3-hour intervals.

The script extracts the temperature and timestamps from the response.

It then converts timestamps into a readable format.

Finally, it plots the temperature values against the corresponding timestamps using Seaborn and Matplotlib.

Where and How This Can Be Used:
This project is ideal for anyone looking to learn or demonstrate real-world applications of Python in data integration and visualization. Some practical uses include:

Educational Projects: Students can use it to understand APIs, JSON data handling, and visualization in Python.

Weather Monitoring Applications: Can be extended into a larger system for tracking and displaying weather data in real-time.

Web Dashboards: The script can be converted into a web-based dashboard using frameworks like Streamlit or Dash for user interaction.

IoT Systems: Integrating this with IoT devices allows automatic responses based on weather predictions, such as in agriculture or smart home systems.

Data Science Practice: A great starting point for beginners in data science to practice working with external data sources and visual analytics.

#OUTPUT

![Image](https://github.com/user-attachments/assets/b317ff18-188d-4367-be9f-1246c4bb075d)
