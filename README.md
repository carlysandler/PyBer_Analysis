# PyBer_Analysis
*Ride-sharing data analysis and DataFrame summary visualition with*: `Jupyter Notebook`, `Python`, `Anaconda`, `Matplotlib`, `NumPy`, `SciPy`
---
## Overview of Analysis
PyBer, the ride-sharing company, requested our expertise in data visualization to help them better improve access to ride-sharing services and determine the most appropriate and economically competitive fare prices for underserved neighborhoods. Specifically, when tasked with determining the correlation between city type and fare amount,  we must create a summary `DataFrame`, which will consisely visualize, in tabular form, how the data differs by city type, on key metrics that measure supply and demand for each city type. Once done with this deliverable, a line graph will be created from PyBer's 2019 ride-sharing data, plotting the relationship between city type and weekly fare amounts (USD$). This analysis will deliniaate the steps taken to complete the two Deliverable mandates, as well as business recommendations to PyBer on how to improve ride acccessibility, based on the results shown below. 

The key variables of interest are as followed. 

Firsly, our index variable: `type`. The three different city types in the US we are analysising are:

  __City Type__:
  - Urban
  - Suburban
  - Rural

Secondly, our column variables--the key "relational" metrics of interest that differ by city type (for ascertaining economic efficiency and ride accessibility):

  __Column Variables: DataFrame__         __Column Variables: Python script__
  - Total Rides                             - `total_rides_by_type`
  - Total Drivers                           - `total_drivers_by_type`
  - Total Fares                             - `total_fares_by_type`
  - Average Fare per Ride                   - `avg_fare_per_ride`
  - Average Fare per Driver                 - `avg_fare_per_driver`

---
### Deliverable 1
The below steps annotate the process of completing the brief for Deliverable 1.
1) Merge the `city_data_df` and the `ride_data_df` using the Pandas `merge()` function, on the shared variable "city", specifying "how" with the parameter `how=left`.
2) Get the column variables from the merged `pyber_data_df` using the `groupby()` function, in conjunction with `sum()` and `count()` methonds.
 - Total Rides
 - Total Drivers
 - Total Fares
3) Use arithmatic division  on our newly initalizated and calculated variables: get the average fare per ride and average fare per driver for each city type.:
 - Average Fare per Ride
 - Average Fare per Driver
4) Create the PyBer summary DataFrame with our five column variables and city type as our index.
5) Clean up and format the DataFrame, removing the index name and making the column outputs viwer-friendly.

*Deliverable 1:*

![pyber_summary_df](https://user-images.githubusercontent.com/77628698/111909494-eaab6b80-8a33-11eb-8c5f-6b81883a993a.png)


---
### Deliverable 2 
The below steps annotate the process of completing the brief for Deliverable 2, which requires us to use two new functions `pivot()` and `resample()` to create a multiple-line graph.
1) Create a new DataFrame with multiple indicies: "type" and "date" using the `groupby()` function on the respective columns of `pyber_data_df`
  - Retrieve total fare amount for each date for each city type.
2) Reset the index and use the pivot function to convert the new DataFrame so that:
 - index = "date"
 - columns = each city "type"
 - values = "fare"
3) Use the loc method on the specified date range, Jan-Apr 2019, to create a new DataFrame and reset the indext to a datetime data type.
4) Apply the `resample()` function to the newly modified DataFrame, to resample the data in weekly bins, instead of in days, and sum up the data to get:
  - Total Fares for each week
5) Graph the resampled DataFrame with `df.plot()` and annotate the y-axis label and title.
  - Use Matplotlib's `"fivethirtyeight"` graph style to present to PyBer's team.  


*Deliverable 2:*

![Total_Fare_by_City_Type](https://user-images.githubusercontent.com/77628698/111909574-39590580-8a34-11eb-9fb3-e2b817ad5305.png)

---
## Results
Looking at the PyBer Summary DataFrame, based on each city type, we can conclude that:
Total Rides (Demand)
- In rural cities, total ride count is 4x lower than the ride count of Urban cities.
- In rural cities, total ride count is 3.5x lower than the ride count of Suburban cities.

Total Drivers (Supply)
- Urban cities' total driver count is 9x higher than that of Rural cities.
- Urban cities' total driver count is 3x higher than that of Suburban cities.
- Suburban cities' total driver count is 6x higher than that of Rural cities.

Total Fares (Pricing given supply and demand)
- Total fares of Urban cities are only 2x higher than total fares of Suburban cities.
 - Note: total rides of Urban cities are 2.6x higher than total rides of Suburban cities
 - Note: total drivers of Urban cities are almost 5x higher than total drivers of Suburban cities.
 - Indication of economic inefficency as the supply and demand for Pyber rides in Urban cities are not equal.

% of Total Rides, Drivers, and Fares for each city type (Urban, Suburban, and Rural) can be visually displayed with the below Pie Charts.
*% of Total Fares by City Type from PyBer.ipynb*
<img width="340" alt="Fig5" src="https://user-images.githubusercontent.com/77628698/111917833-72a36c80-8a58-11eb-8f68-d11020b9f915.png">


*% of Total Rides by City Type from PyBer.ipynb*
<img width="380" alt="Fig6" src="https://user-images.githubusercontent.com/77628698/111917826-6cad8b80-8a58-11eb-83b0-03504752a77a.png">

*% of Total Drivers by City Type from PyBer.ipynb*
<img width="346" alt="Fig7" src="https://user-images.githubusercontent.com/77628698/111917863-84850f80-8a58-11eb-9bdc-4cb94473a80b.png">

Average Fare per-Ride
- The avg fare/ride price in Rural cities is about $10 more than that of Urban cities, and $6 more than that of Suburban cities.
- With 

Average Fare per Driver
                           
  - Total Drivers                          
  - Total Fares                             
  - Average Fare per Ride                   
  - Average Fare per Driver                 

- b
- b
- b
- b

Looking at the "Total Fare by City Type" muliple lign graph, we can clude that:
-b
0b
-b
-b




*PyBer Ride-Sharing Data (2019) from PyBer.ipyng*
<img width="800" alt="PyBer_Ride_Sharing_Data_2019" src="https://user-images.githubusercontent.com/77628698/111917698-d11c1b00-8a57-11eb-9011-9b07f096b826.png">



---
### Business Recommendations 




