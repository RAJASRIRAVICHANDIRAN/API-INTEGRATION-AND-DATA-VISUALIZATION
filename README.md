# PYTHON INTERSHIP

*COMPANY*:CODTECH IT SOLUTIONS

*NAME*:R.Rajasri

*INTERN ID*:CT04DA237

*DOMAIN*:PYTHON PROGRAMMING

*DURATION*:4 WEEKS

*MENTOR*:NEELA SANTHOSH
#TASK1:# API-INTEGRATION-AND-DATA-VISUALIZATION
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

#OUTPUT OF TASK1

![Image](https://github.com/user-attachments/assets/b317ff18-188d-4367-be9f-1246c4bb075d)

#DESCRIPTION OF TASK2
This Python script is designed to automate the process of reading data from a CSV file, performing basic analysis on a specific column, and generating a professional-looking PDF report. It leverages two powerful Python libraries: pandas for data handling and fpdf for creating PDF documents. This kind of script is especially useful in business and data analytics environments where regular reporting is required.

📁 Step-by-step Explanation of the Code
Importing Libraries
The script begins by importing two essential libraries:

pandas: A widely used data manipulation library, ideal for handling structured data like CSV files.

fpdf: A simple PDF generation library in Python that allows for text, tables, and graphical elements to be written into a PDF document.

Specifying File Path
The path to the CSV file is set using a raw string format (r"E:\sample_data.csv"). This is important on Windows systems to avoid issues with backslashes being interpreted as escape characters. This path points to the sample_data.csv file stored in the E: drive of the user's system.

Reading the CSV File
The pandas.read_csv() function is used to read the CSV file into a DataFrame (data). A DataFrame is a 2D data structure that allows easy manipulation and analysis of tabular data.

Performing Data Analysis
The script focuses on analyzing a single column named "Sales":

It calculates the mean (average) using .mean()

Finds the maximum value using .max()

And identifies the minimum value using .min()

These statistics are useful to quickly summarize the dataset and understand trends in the data.

Creating the PDF Report
The PDF creation process begins with:

Creating a FPDF object

Adding a page using add_page()

Setting the font with set_font() (Arial, size 12)

Then, the script writes the report content:

The title "Sales Report" is added and centered using cell()

A line break is inserted with ln(10)

The average, maximum, and minimum sales values are each added as separate lines

Saving the PDF
The output() method is called with the filename "report.pdf". This generates a PDF file in the same directory where the script is run. The file contains all the formatted statistics from the analysis.

Final Output
A message "✅ PDF report generated as report.pdf" is printed to confirm successful completion.

🎯 Use Cases
Weekly/monthly business sales summaries

Automated school reports for student scores

Financial trend tracking

Any domain where numerical analysis and reporting are essential

✅ Conclusion
This Python script demonstrates the power of combining data analysis with automation. It is an efficient solution for generating readable and portable reports. By modifying the CSV path or column name, the same code can be reused for various datasets and reporting needs.
#OUTPUT TASK2

