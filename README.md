# Ford-GoBike-System-Data-Exploration-and-Visualization

**AIM :** Investigate how the duration of trips changes with respect to DateTime and customer type.

**Ford GoBike System Data:** This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.


## **Dataset Overview**

The Ford-GoBike dataset has 183412 records and 16 columns. 

The datatypes distribution is as follows:

|Column                   |Datatype|
|-------------------------|--------|
|duration_sec             |int64   |
|start_time               |int64   |
|end_time                 |int64   |
|start_station_id         |int64   |
|start_station_name       |int64   |
|start_station_latitude   |int64   |
|start_station_longitude  |int64   |
|end_station_id           |int64   |
|end_station_name         |int64   |
|end_station_latitude     |int64   |
|bike_id                  |int64   |
|user_type                |int64   |
|member_birth_year        |int64   |
|member_gender            |int64   |
|bike_share_for_all_trip  |int64   |


`start_station_id`, `start_station_name`, `end_station_id`, `end_station_name`, `member_birth_year` and `member_gender` has got missing values.

## **Steps Taken**

For this project, I set to find out the duration when most bikes are used by which kind of customers. My main focus was on age, time, user type and gender. 

### Step-wise Approach

- I obtained and loaded the dataset.

- I did the cleaning the data i.e data wrangling, which involved the following steps:
    * Removed the null values.
    * Conversion of datatypes.
    * Conducting various transformations and feature engineering on the dataset. 
    
- visualization and insights communication.

## **Summary of Findings**
<hr>

## Univariate Analysis
<hr>

1.) The following observations were made from `duration_sec`

    - It's highly skewed to the right and therefore needs a transformation

    - It's unimodal

2.) The following was observed from `start_of_the_week`

    - Most trips are made on weekdays with Thursday leading 

    - Few trips were made on weekends.

3.) Observation made from `Hour`

    - Most trips are made between 8am and 6pm

4.) Observations from `start_day_of_the_month`

    - Most trips were made on 28th february 
    
    - Least on 9th february

5.) Observations from `member_birth_year`

    - Most riders were born in 1988 

6.) Observations from the `customer_age`

    - The `customer_age` feature contains several outliers that needs to be removed.

7.) Observations from the `customer_gender`

    - The `customer_gender` feature shows more male riders.

8.) Observations from the `user_types`

    - Majority of the customers are subscribers.
<hr>




## Bivariate Analysis
<hr>

1.) `customer_age` and time spent

    - Convert `duration_sec` from seconds to hours and visualize against customer age

    - Most young people between of approximately 20 and 45 years cycle for more hours than other ages

2.) Checking for trends in `Customer_age` and hours spent riding

    - Males aged 30-45 used more bikes between the 0 and 5th hour

3.) Checking for duration of trips made on weekdays vs those made on weekends

    - Longest rides were on the weekend.

    - Longest weekday rides were on Monday

4.) Count of gender and `user_type`

    - More subscriber males are enrolled in biking

<hr>



## Multivariate Analysis
<hr>

1.) Distribution of trip duration by user Type and gender

    - There's a dense user concentration below 5hr mark

2.) `user_type` trip duration*

    - From the two visuals above, both the customer and subcriber show similar trend

3.) `user_type` distribution in comparison to 'customer_age' and `duration_sec` in `hours`

    - From the distribution most users spend less than 5 hours biking.

<hr>




## Key Insights for Presentation

Most bike users are subscribers and most hiring is done between 8am and 5pm.

Majority of the bikers are males with age ranging from 20-40 years of age.

Most bikes are used in rush hours. 

The users may be working class and hire bikes to and from work.

