# US-Domestic-Flight-Performance-Dashboard
In this project as part of the IBM Data Analyst Certification, i created an interactive dashboard that analysis the performance of the reporting airline to improve fight reliability thereby improving customer reliability.

# Airline Data Dashboard
The interactive web-based dashboard for visualising and analyzing data related to domestic airline flights. It's built using Dash, a web framework for Python. The dashboard was created through the following steps: 

1. Importing Libraries: 
All the essential python libraries required were imported, this including Pandas for data manipulation, Dash for creating web applications, Plotly for data visualization, and more.

2. Creating a Dash Application: 
A Dash application was initialised with the line "app = dash.Dash(__name__)". This is where the layout and functionality of our web application is defined.

3. Reading Data: 
The airline data was loaded from a CSV file using Pandas. This data contains information about airline flights, including details like the month, reporting airline, and various types of delays.

4. Layout Setup: 
Here, the structure of the web application was defined. two dropdwons were created for users to select the type of report and the year they're interested in. Additionally, an empty spaces (placeholders) was included where the graphs will be displayed.

5. Callback Function: 
This is a crucial part of the web application. the callback function was defined  with the "@app.callback decorator". When users interact with the web application this function is triggered. It calculates the data needed to create graphs based on the user's selections.

If the user chooses "Yearly Airline Performance" ("OPT1"), the function computes data for various graphs, including those related to monthly flight cancellations, average flight times, diverted airport landings, and more. These computed graphs are then returned as components and displayed on the web page.

<img width="900" alt="Screenshot 2023-11-17 at 20 12 44" src="https://github.com/moheebprojects/US-Domestic-Flight-Performance-Dashboard/assets/125134551/4080a0fe-a158-4516-a00f-0c80ce273bb1">


Alternatively, if "Yearly Airline Delay Report" ("OPT2") is selected, the function calculates data for different types of delays (e.g., carrier delay, weather delay) and presents these computed graphs.

<img width="900" alt="Screenshot 2023-11-17 at 20 13 01" src="https://github.com/moheebprojects/US-Domestic-Flight-Performance-Dashboard/assets/125134551/19e6bad1-d768-48a5-b833-95933b811077">


6. Run the App
To launch the web application, a block of code that runs it. If this script is executed as the main program, the "app.run_server(debug=True)" line starts the web application and serves it locally.

In summary, this script sets up a web-based dashboard that allows users to choose between two types of reports related to domestic airline flights. Depending on the report type and year selected, the script calculates and displays relevant data visualizations, such as graphs and charts, to offer insights into airline performance and delays. You can access this web application by running the script.
