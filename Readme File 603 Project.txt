<h1>Installing the required Libraries</h1>
<p>1. Importing the required packages for data accessing,
   analysis and visualization</p>
<p>2. Import the required libraries required for regression</p>
<h1>Idenitifying Data issues</h1>
The next steps we will check if for each important feature if there are any data issues or issing values. We are considering data from 2014 t0 2020. 2013 data is exempted from analysis based on previous research work on this data and literature review. 2021 data was incomplete and continously changing during the course of this project, so it is removed from the analysis
<h1>Steps invloved </h1>
<p>1.Checking if there are any records with missing trip_start_timestamp</p>
<p>2.Checking if there are any records with missing trip_end_timestamp </p>
<p>3.Checking if there are any records where the trip start time is greater than trip end time</p>
<p>4.Checking for latitude and logitude missing records</p>
<p>5.Checking for distribution and existence of other useful features for latitude and logitude missing records</p>
<p>6.Checking for trips that lasted more than 3 hours</p>
<p>7.Checking for trips that have trips total amount less than $3.25 (which is official minimum fare for any trip)</p>
<p>8.Checking distribution of trip miles, most of the records have less than 100 mile. Longest route which is from OHare to Hegewisch is only 50 miles considering double the 50 it should be more than 100 for trips with in chicago</p>
<h1>Preparing the filter which will be used for all the queries in this notebook</h1>
We are going to fiter all the records which we identified as issues in the above section.
<p>The conditions are as followes</p>
<p>1. Year of Pickup time should be between 2014 and 2020</p>
<p>2. Pickup latitude and logitudes should not be NULL</p>
<p>3. Trip end time stamp should not be NULL</p>
<p>4. Trip start time should be less than trip end time</p>
<p>5. Trip duration should be less than or equal to 180 minutes (3 hours)</p>
<p>6. Pickup and dropoff community areas should be present</p>
<p>7. Trip total amount should atleast be $3.25</p>
<p>8. Trip miles should be less than or equal to 100 miles</p>
<h1>Visualizations</h1>
<p>1.Visualization to show trips per day over the year</p>
<p>2.Number of rides per month for each year</p>
<p>3.Average trips per hours for both weekdays and weekends</p>
<p>4.Bar plot to show the number of rides per week</p>
<p>5.Plotting the number of active taxis for each month of 2020</p>
<p>6.Plotting both travel time and distances</p>
<p>7.Plotting average wait time</p>
<p>8.Plotting average trips per taxi in a day</p>
<p>9.Plotting avarage number of trips per day for Far Southeast side areas</p>
<p>10.Plotting the avarage number of dropoff for Pullman and South Shore areas</p>
<h1>MongoDB</h1>
<p>Getting full data with the required features for prediction</p>
<p>1.Transferring this data to mongodb</p>
<h1>MongoDB -> Jupyter Notebook Using Pyspark</h1>
<p>1.Install the required libraries</p>
<p>2.Create a database</p>
<p>3.Import pyspark libraries</p>
<p>4.Using VectorAssembler combine the columns to execute the data in Linear regression model</p>
<h1>Linear Regression</h1>
<p>1.Train the model</p>
<p>2.Executing the test model</p>
<p>3.Finding the Root Mean Squared Error(RMSE)</p>
<p>4.Finding the R2 score</p>
