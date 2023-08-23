Climate Analysis and API Development
This project provides a climate analysis of a database containing weather data for a specific location. The database includes temperature, precipitation, and station information. Additionally, a Flask API has been developed to provide access to this climate data through a set of defined routes.

Project Structure
  Resources: This folder contains all the necessary data for the analysis, including the database file (hawaii.sqlite).

  climate.ipynb: This Jupyter Notebook file contains the initial climate analysis and data exploration. Python, SQLAlchemy ORM     queries, Pandas, and Matplotlib have been used to perform this analysis. It includes data visualization and queries on           temperature and precipitation data.

  app.py: This script is where the Flask API has been developed. It defines various routes that allow users to access climate      data and temperature statistics. The available routes and their descriptions are listed below.

Routes in the Flask API
    /: The homepage, which lists all available routes.

    /api/v1.0/precipitation: Returns a JSON list of precipitation data for the last 12 months.

    /api/v1.0/stations: Returns a JSON list of stations from the dataset.

    /api/v1.0/tobs: Returns a JSON list of temperature observations for the previous year from the most active station.

    /api/v1.0/<start>: Calculates and returns a JSON list of the minimum temperature (TMIN), average temperature (TAVG), and         maximum temperature (TMAX) for a specified start date. You can provide an actual date in the <start> parameter.

    /api/v1.0/<start>/<end>: Calculates and returns a JSON list of TMIN, TAVG, and TMAX for a specified date range (inclusive of     both start and end dates). You can provide actual dates in the <start> and <end> parameters.

Usage
To use this project, follow these steps:

Access the Resources folder to find the database file and data.

Review the climate.ipynb notebook for the initial climate analysis.

Run the app.py script to start the Flask API.

Access the routes listed in the API to retrieve climate data and temperature statistics. For routes /api/v1.0/<start> and /api/v1.0/<start>/<end>, provide actual dates in the URL parameters to get temperature statistics for those dates.

References
Menne, M.J., I. Durre, R.S. Vose, B.E. Gleason, and T.G. Houston, 2012: An overview of the Global Historical Climatology Network-Daily Database. Journal of Atmospheric and Oceanic Technology, 29, 897-910, https://journals.ametsoc.org/view/journals/atot/29/7/jtech-d-11-00103_1.xmlLinks to an external site.
