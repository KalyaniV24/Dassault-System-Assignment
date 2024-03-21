# Dassault-System-Assignment

# Question no. 1 
Analyzing Correlation between Blood Group Type, Gender, and Medical Condition:

This documentation outlines the process of analyzing the correlation between blood group type, gender, and medical condition using Python. The analysis is performed on a healthcare dataset provided in the attached Healthcare_Data.zip file.

Prerequisites:
 - Before proceeding, ensure that you have the following installed:
 - Python (with necessary libraries: pandas, matplotlib, seaborn)
You can install the required packages using pip:

"pip install pandas matplotlib seaborn"

Step-by-Step Guide
1. Dataset Exploration:
- Extract the data from the Healthcare_Data.zip file and load it into a Pandas DataFrame.
- Explore the dataset to understand its structure and contents.

2. Data Visualization:
- Use Python libraries such as Matplotlib and Seaborn to create plots for visualization.
- Plot the relationship between blood group type, gender, and medical condition to determine if there is any correlation.

3. Correlation Analysis:
- Analyze the plotted data to identify any patterns or trends.
- Look for correlations between blood group type, gender, and medical condition.
- Use statistical techniques or visual inspection to determine the strength and significance of the correlations.

4. Interpretation:
- Interpret the results obtained from the correlation analysis.
- Draw conclusions about the relationship between blood group type, gender, and medical condition based on the analysis.

Conclusion:

This documentation provides a step-by-step guide for analyzing the correlation between blood group type, gender, and medical condition using Python. By following the outlined steps, you can gain insights into the relationships between these variables and better understand their impact on healthcare outcomes.

# Question no. 2

Creating a Flask Web Application for Healthcare Data Analysis:

This documentation outlines the process of creating a web application using Flask, a Python web framework, to analyze healthcare data. The application allows users to input their name, gender, and blood group, and then provides them with the corresponding medical condition they are at risk of. Additionally, the application stores the user-entered data in a separate CSV file.

Prerequisites:
Before proceeding, ensure that you have the following installed:

- Python (with pip)
- Flask
- pandas
- flask-ngrok (for running Flask application in Jupyter Notebook)

You can install the required packages using pip:

"pip install Flask pandas flask-ngrok"

Step-by-Step Guide
1. Dataset Preparation:
- Obtain the healthcare dataset containing information about patients, including their names, gender, blood group type, and medical conditions.
- Ensure the dataset is in a CSV format and contains relevant columns.

2. Flask Application Setup:
- Create a new Python file (e.g., app.py) to contain the Flask application code.
- Import necessary modules:

"from flask import Flask, request

from flask_ngrok import run_with_ngrok

import pandas as pd"

3. Load Dataset:
- Load the healthcare dataset into a Pandas DataFrame:

"data = pd.read_csv('healthcare_dataset.csv')"

4. Define Flask Routes:
Set up routes for the Flask application:
- Define a route to display the HTML form for user input (/ route).
- Define a route to handle form submission and display the result (/ route with POST method).
  
5. HTML Form Creation:
- Create an HTML form for user input within the Flask application code.
- Use the index() function to render the HTML form when users access the root URL (/).

6. Processing User Input:
- Define a function (submit()) to process the user-entered data when the form is submitted.
- Extract user input (name, gender, blood group) from the form using Flask's request object.
- Use the user input to determine the corresponding medical condition from the dataset.

7. Display Result:
- After processing the user input, display the result (medical condition) to the user.
- Generate HTML content dynamically based on the result and return it to the user.

8. Store User Data:
- Store the user-entered data (name, gender, blood group) in a separate CSV file.
- Append the user data to the CSV file each time a new submission is made.

9. Run the Flask Application:
- Start the Flask application by running the Python script (Question2 app.py).
- The application will be accessible locally at a URL provided by ngrok.

Conclusion:

This documentation provides a step-by-step guide for creating a Flask web application to analyze healthcare data. Users can input their information to determine the medical condition they are at risk of, and their data is stored for future reference.
