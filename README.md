**Project Overview**

This project focuses on climate data analysis using SQLAlchemy, Pandas, Matplotlib, and Flask. You'll analyze weather patterns in Honolulu, Hawaii, and build a climate API to serve insights derived from the dataset.


Prerequisites
Ensure you have the following installed:
- Python 3.7+
- Jupyter Notebook
- Flask
- SQLAlchemy
- Pandas
- Matplotlib

**Part 1: Climate Data Analysis**
Using SQLAlchemy and Pandas, you will explore the climate dataset.

Steps:
1. Connect to SQLite Database
- Use create_engine() to connect to hawaii.sqlite.
- Reflect tables using automap_base().
- Reference station and measurement tables.
- Create a session to interact with the database.

2. Precipitation Analysis
- Retrieve precipitation data for the last 12 months.
- Store results in a Pandas DataFrame.
- Sort values by date.
- Plot precipitation trends.
- Print summary statistics.

3.Station Analysis
- Count the number of weather stations.
- Identify the most active station.
- Calculate min, max, and average temperatures.
- Retrieve the last 12 months of temperature data.
- Plot results as a histogram.
- Close the Database Session

**Part 2: Flask API**
Create a Flask web application to serve climate data through API routes.

Available Routes:
- Homepage (/): Displays available API routes.
- Precipitation (/api/v1.0/precipitation): Returns JSON of precipitation data for the last 12 months.
- Stations (/api/v1.0/stations): Returns a list of weather stations.
- Temperature Observations (/api/v1.0/tobs): Returns temperature observations from the most active station for the last year.
- Temperature Statistics (/api/v1.0/<start> and /api/v1.0/<start>/<end>):

Running the Flask App
- To start the Flask API, run: python app.py
- Then access http://127.0.0.1:5000/ in your web browser.
