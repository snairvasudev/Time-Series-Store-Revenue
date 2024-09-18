Your task, is to create a model to predict the revenue of an online retailer - let's call them ABC-Retail. We have provided you with the following data to achieve this:
 
Order numbers
Two columns: date and order_number
When consumers place orders on ABC-Retail's website, this produces a sequential order number, which can be helpful for estimating the number of purchases a consumer made. This is the information stored in the table.
For example, the first two rows show an order number of 33841906 on 7 January 2018, and 34008921 on 22 January 2018. If we take the difference between the two values, you will get 167,015. This implies that there were around 167,000 orders between those two dates.
Other notes:
We do not have an order number for every single day, there are gaps in the data.
The order numbers should always increase over time (because order number only goes up), but the data has not been cleaned! and there are some bad datapoints that will need to be dealt with.
 
Transaction data
Three columns: date, total_spend_index, and weekly_active_users_index.
The total_spend_index gives an indexed estimate of the total volume of purchases that consumers made on a given day.
The weekly_active_users_index provides an indexed estimate of the number of users in our transaction data.
Other notes:
Both columns are indexed to a value of 100 on 20 May 2020
There are no gaps in this data, but you will notice the number of active users is quite low in earlier time periods, so you would expect the values in 2018 or earlier to be quite noisy.
 
Reported data
Four columns: period, start_date, end_date and revenue_index
The period shows a label for the period in question - the label is arbitrary.
The start_date and end_date show when the period in question began and ended (the dates are inclusive)
The revenue_index shows the revenue the company made between the start_date and end_date
Other notes:
The revenue has been indexed to the value in 2018 Q1
The number of days in each period is NOT identical
 
Data preparation and modelling
Your goal is to build a model to predict ABC-Retail's revenue_index. You should train your model on any number of the reported values up-to-and-including 2022 Q3, and evaluate the model on 2022 Q4. Please report some metrics on your model performance such as the in-sample R-squared, and percentage error on the out-of-sample test point.
 
You will need to clean and process the data in order_numbers and transaction_data to create features for your model to use.
