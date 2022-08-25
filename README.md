# Feature_Engineering_Core

In this exercise you will be working with data about bike share rentals.  You can download the data here.

Your task is to engineer some new features to try to improve a mode's ability to predict the total number of bike share rentals during a given hour of the day.

1. Import the data the drop the 'casual' and 'registered' columns.  These are redundant with your target, 'count'.  



2. Transform the 'datetime' column into a datetime type and use it to create 3 new columns in the data frame containing the:

  1. Name of the Month
  2. Name of the Day of the Week
  3. Hour of the Day

   Make sure all 3 new columns are 'object' datatype so they can be one-hot encoded later.  

   Drop the 'datetime' and 'season' columns.  These are now redundant.



3. The temperatures in the 'temp' and 'atemp' column are in Celsius.  Use `.apply()` to convert them to Fahrenheit.



4. Create a new column, 'temp_variance' that is the difference between 'temp' and 'atemp'.  Drop the 'atemp' column.



Optional: 
Use a predictive model of your choice and try to predict the 'count' of hourly bikeshare users with both the original features and the engineered feature set you just created.  

Remember to drop the 'casual' and 'registered' columns from both versions before modeling.

Did these feature engineering choices improve your ability to predict the 'count'?
