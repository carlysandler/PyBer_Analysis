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
3) Use arithmatic division  on our newly initalizated and calculated variables:
 - Total Rides
 - Total Drivers
 - Total Fares
To get the average fare per ride and average fare per driver for each city type.
4) Create the PyBer summary DataFrame with our five column variables and city type as our index.
5) Clean up and format the DataFrame, removing the index name and making the column outputs viwer-friendly.

*Deliverable 1:*

![pyber_summary_df](https://user-images.githubusercontent.com/77628698/111909494-eaab6b80-8a33-11eb-8c5f-6b81883a993a.png)


---
### Deliverable 2 
The below steps annotate the process of completing the brief for Deliverable 2.
1)

*Deliverable 2:*

![Total_Fare_by_City_Type](https://user-images.githubusercontent.com/77628698/111909574-39590580-8a34-11eb-9fb3-e2b817ad5305.png)

---
## Results



---
## Concluding Statements



---
### Business Recommendations 




