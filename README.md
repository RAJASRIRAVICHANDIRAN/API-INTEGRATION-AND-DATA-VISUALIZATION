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

![Image](https://github.com/user-attachments/assets/f21373c9-ebdb-4afa-9ffd-64c26b5aecd7)
##TASK3

This Python script creates a simple AI chatbot using Natural Language Processing (NLP), which can respond to user queries in an interactive manner. It leverages the NLTK (Natural Language Toolkit) library, a popular Python library for working with human language data, and specifically uses the nltk.chat.util.Chat class to build the chatbot. The chatbot is capable of recognizing user inputs, matching them with predefined patterns, and generating appropriate responses. This type of chatbot is relatively simple but serves as a great introduction to more advanced chatbot development techniques.

Key Components of the Program
Libraries Used:

nltk (Natural Language Toolkit): This is a powerful library used for working with text data in Python. It provides easy-to-use interfaces for text processing tasks like tokenization, parsing, and more. In this program, the chatbot utilizes NLTK's Chat class, which helps match user inputs with predefined responses based on regular expressions.

reflections: This is an inbuilt dictionary in nltk.chat.util that reflects pronouns and personal pronouns, like changing "I" to "you" and "me" to "you". It makes the chatbot's responses feel more conversational and natural.

Pattern-Response Matching:

The core of this chatbot's functionality lies in pattern matching. The chatbot uses regular expressions to identify specific phrases in user input. If a user types a greeting like "hi" or "hello", the chatbot responds with a matching phrase like "Hello!" or "Hi there!". Similarly, if the user asks about the chatbot's name, the chatbot has a response like "I'm your friendly chatbot."

The patterns are defined as regular expressions (e.g., r"hi|hello|hey"), and each pattern corresponds to one or more possible responses (e.g., ["Hello!", "Hi there!", "Hey!"]).

Chatbot Structure:

The chatbot is initialized with a list of predefined patterns and responses. The Chat class uses this list to match user inputs with the appropriate responses.

The start_chat function handles the interactive conversation. It keeps asking for user input, processes the query, and provides a response. If the user inputs "quit", the conversation ends, and the chatbot bids farewell.

Interaction and Input:

The chatbot runs in a loop, waiting for the user’s input. Upon receiving user input, the chatbot tries to match it with one of the predefined patterns. If it finds a match, it responds with the corresponding answer.

For instance, if a user says "hello", the chatbot will respond with a greeting, like "Hi there!". If the user says something that doesn’t match any patterns, the chatbot will respond with a default message: "Sorry, I don't understand that."

Ending the Conversation:

To end the conversation, the user simply types "quit" or "exit". The program will break the loop and display a farewell message, indicating the end of the session.

Flow of the Program:
The script begins by importing the necessary libraries.

It defines a set of patterns and responses, which are matched during the chat.

The start_chat function runs the interactive loop, waiting for user input and providing a response based on the matched pattern.

The chatbot responds with one of the predefined answers or with a default response when no match is found.

The loop continues until the user types "quit" or "exit", at which point the conversation ends.


output for task 3:
![Image](https://github.com/user-attachments/assets/5094e014-3117-40ea-bc1b-ebf17e9215b9)

##TASK4
The program presented above demonstrates the process of building a text classification model using scikit-learn. It focuses on classifying text messages as either 'spam' or 'ham' (non-spam), utilizing a simple machine learning pipeline. This approach is common in various natural language processing (NLP) tasks where the goal is to classify textual data into different categories. In this case, we aim to distinguish between spam and non-spam messages.

Step 1: Dataset Creation
For the demonstration, a sample dataset is created manually within the code. The dataset consists of ten text messages that are either labeled as 'ham' (non-spam) or 'spam'. The messages cover a wide range of content, such as friendly messages ("Hello, how are you?") and promotional content ("Free money now!!!"). This dataset is then stored in a pandas DataFrame, which is a widely-used data structure for handling tabular data in Python.

The creation of a custom dataset is essential for the development of a machine learning model, as it allows users to test the model on their specific data. In real-world applications, these datasets are typically much larger and more complex.

Step 2: Data Preprocessing
The next critical step is transforming the raw text data into a format that a machine learning model can process. This is done using CountVectorizer, which is part of the scikit-learn library. The CountVectorizer converts the text into a matrix of token counts, which is often referred to as the bag-of-words model. In this model, each word in the text is treated as a feature, and the matrix represents the occurrence of each word in the given messages.

Additionally, common words (known as stop words) are excluded from the feature set using the stop_words='english' parameter. These stop words include common terms such as "the", "is", "and", etc., which are usually not useful for text classification tasks.

Step 3: Label Encoding
The next step involves encoding the labels (i.e., 'ham' and 'spam') into numerical values, since machine learning models typically operate on numerical data. The labels 'ham' and 'spam' are mapped to 0 and 1, respectively, using the map() function of pandas. This binary encoding is essential for training the model.

Step 4: Train-Test Split
Once the data is preprocessed, the next step is to divide the dataset into training and testing sets. This is done using train_test_split from scikit-learn, where 80% of the data is allocated for training and the remaining 20% is set aside for testing. This split is critical to assess the model's ability to generalize to unseen data.

Step 5: Model Training
A Logistic Regression model is chosen for this task, as it is a simple yet effective classification algorithm. Logistic regression is a linear model that is often used for binary classification tasks. In this case, it predicts whether a message is "ham" (0) or "spam" (1). The model is trained using the fit() method on the training data (i.e., the text features and their corresponding labels).

Step 6: Model Prediction
Once the model is trained, it is used to predict the labels for the test set. The predicted labels are compared against the actual labels to evaluate the model's performance.

Step 7: Model Evaluation
The performance of the model is evaluated using two key metrics:

Classification Report: This report includes precision, recall, and F1-score for both classes, 'ham' and 'spam'. Precision measures the accuracy of positive predictions, recall measures how well the model identifies the positive class, and F1-score is the harmonic mean of precision and recall, providing a balance between them.

Confusion Matrix: A confusion matrix is a table used to evaluate the performance of a classification algorithm. It shows the number of true positives, true negatives, false positives, and false negatives. This matrix helps visualize how well the model is distinguishing between the classes.

Step 8: Visualization
Finally, the confusion matrix is visualized using a heatmap generated by seaborn, which provides a clear, easy-to-interpret visualization of the model's performance. The heatmap shows the actual vs predicted classifications, making it easier to see how well the model distinguishes between 'ham' and 'spam' messages.

OUTPUT:
