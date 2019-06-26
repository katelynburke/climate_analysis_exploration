### Surf's Up! - Advanced Data Storage and Retrieval 

#### Step 1 - Climate Analysis and Exploration

To begin, use Python and SQLAlchemy to do basic climate analysis and data exploration of your climate database. 

All of the following analysis should be completed using SQLAlchemy ORM queries, Pandas, and Matplotlib.

Use SQLAlchemy create_engine to connect to your sqlite database.

Use SQLAlchemy automap_base() to reflect your tables into classes and save a reference to those classes called Station and Measurement.

#### Precipitation Analysis

Design a query to retrieve the last 12 months of precipitation data.

Select only the date and prcp values.

Load the query results into a Pandas DataFrame and set the index to the date column.

Sort the DataFrame values by date.

Plot the results using the DataFrame plot method.

Use Pandas to print the summary statistics for the precipitation data.

#### Station Analysis

Design a query to calculate the total number of stations.

Design a query to find the most active stations.

List the stations and observation counts in descending order.

Which station has the highest number of observations?

Design a query to retrieve the last 12 months of temperature observation data (tobs).

Filter by the station with the highest number of observations.

Plot the results as a histogram with bins=12.

#### Step 2 - Climate App

Now that you have completed your initial analysis, design a Flask API based on the queries that you have just developed.

Use FLASK to create your routes.

Convert the query results to a Dictionary using date as the key and prcp as the value.

Return the JSON representation of your dictionary.

Return a JSON list of stations from the dataset.

Return a JSON list of Temperature Observations (tobs) for the previous year

Return a JSON list of the minimum temperature, the average temperature, and the max temperature for a given start or start-end range.

When given the start only, calculate TMIN, TAVG, and TMAX for all dates greater than and equal to the start date.

When given the start and the end date, calculate the TMIN, TAVG, and TMAX for dates between the start and end date inclusive.
