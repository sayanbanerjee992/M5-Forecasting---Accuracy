# M5-Forecasting---Accuracy
M5 Forecasting - Accuracy is a Sales forecasting project using Machine Learning. This is a Machine Learning Regression Problem.

<h2> What is Sales Forecasting?</h2>

<p>
Sales forecasting is the process of estimating future revenue by predicting the amount of product or services a sales unit (which can be an individual salesperson, a sales team, or a company) will sell in the next week, month, quarter, or year.
</p>

<h2> Problem Statement</h2>

<p>
Forecating sales is essential for the companies for example, investing new methodoligies to increase their revenue for their products which may account for low sales in the future through promotions/discounts etc.. Hence for the established businesses it becomes important to <b> forecast the future sales accurately.<b>
</p>
  
  
  <h2>  Business objectives and constraints. </h2>
  
  *   High Interpretability as we need to know what are the
important factors contributed in forecasting accurately.

*   No strict low latency as we need to forecast sales
on a daily basis as compared to minute or hourly basis.


  <h3>  Data Overview </h3>
  
  <h4>The M5 dataset constists of 3 files </h4>
<b>Source- </b> https://www.kaggle.com/c/m5-forecasting-accuracy/data

1.   Calender.csv - Contains information about the dates the products are sold.
    *   date: The date in a “y-m-d” format.
    *   wm_yr_wk: The id of the week the date belongs to.
    *   weekday: The type of the day (Saturday, Sunday, …, Friday).
    *   wday: The id of the weekday, starting from Saturday.
    *   month: The month of the date.
    *   year: The year of the date.
    *   event_name_1: If the date includes an event, the name of this event.
    *   event_type_1: If the date includes an event, the type of this event.
    *   event_name_2: If the date includes a second event, the name of this event.
    *   event_type_2: If the date includes a second event, the type of this event.
    *   snap_CA, snap_TX, and snap_WI: A binary variable (0 or 1) indicating whether the stores of CA, TX or WI allow SNAP  purchases on the examined date. 1 indicates that SNAP purchases are allowed.
  
  
  
  
2.  sell_prices.csv - Contains information about the price of the products sold per store and date.

    *   store_id: The id of the store where the product is sold
    *   item_id: The id of the product.
    *   wm_yr_wk: The id of the week.
    *   sell_price: The price of the product for the given week/store. The price is provided per week (average across seven days). If not available, this means that the product was not sold during the examined week. Note that although prices are constant at weekly basis, they may change through time (both training and test set).  




3.   sales_train_validation.csv - Contains the historical daily unit sales data per product and store.

    *   item_id: The id of the product.
    *   dept_id: The id of the department the product belongs to.
    *   cat_id: The id of the category the product belongs to.
    *   store_id: The id of the store where the product is sold.
    *   state_id: The State where the store is located.
    *   d_1, d_2, …, d_i, … d_1941: The number of units sold at day i, starting from 2011-01-29. 
  
  
  <h3> Type of Machine Learning Problem </h3>
  
  <p>
The problem we are solving is a time series problem which we can transform it into supervised learning problem by performing Feature engineering on the raw time series data. Then we can use these features as input variables and 'sales of the item' as output variable (Real number) and solve the problem of forecating using Machine learning Regression models.     
</p>
  
  <h3>  Performance Metric</h3>
  
  * RMSE 
    
* R-Square Score
  
  <h3> Kaggle Score </h3>
  ![kaggle_score](https://user-images.githubusercontent.com/65183364/155803757-49848ab2-5138-4cf3-84b5-61bae2338bc7.png)
