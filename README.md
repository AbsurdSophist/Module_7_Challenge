# Module_7_Challenge
In this activity, we built a financial database and web applicatoin by using SQL, Python, and the Voila library. Using Jupyter lab, we were able to create an application that analyzed hypothetical ETF data that a SQL database stored. 

After importing the required libraries and creating our temporary sqlite database and database engine, we used a SQL SELECT statement that read in a single asset from the ETF portfolio. We then created a DataFrame from the resulting query, and created an interactive visualization showing average daily returns and cumulative daily returns of the single asset using hvplot. 

We then used conditional statements, and made use of the LIMIT and ORDER BY statements to create additional dataframes that highlighted specific metrics from the single asset. Doing so potential allows an end user to quickly access relevant metrics with optimized efficiency.

We subsequently created a new dataframe containing data from all assets in our ETF portfolio, by writing a SQL query that joined all tables on the "time" column. Doing so gave a convenient way to view and analyze the data of the entire portfolio. Next, we created a DataFrame to show the averages of the daily return values across all assets. We assumed that the weights of the assets were equal, though if this were not the case this would be a simple change to the code. Having created this new dataframe, we now could calculate the cumulative returns of the ETF portfolio by creating a new dataframe using the cumprod() function, and accessing the final entry in the resulting dataframe. We then used hvplot to create a visualize of cumulative return values.

Using the Voila library, we were able to deploy our notebook as a web application locally. Please see screenshots below displaying how the web application appeared. 
<img width="1373" alt="Voila Screenshot 1" src="https://user-images.githubusercontent.com/60553699/113494576-519e3b00-949e-11eb-9ee9-68a575be95f7.png">
<img width="1373" alt="Voila Screenshot 2" src="https://user-images.githubusercontent.com/60553699/113494578-5367fe80-949e-11eb-9ba2-bd0c157a9e40.png">
<img width="1373" alt="Voila Screenshot 3" src="https://user-images.githubusercontent.com/60553699/113494579-55ca5880-949e-11eb-9bc6-8c1e9a2355e8.png">
<img width="1373" alt="Voila Screenshot 4" src="https://user-images.githubusercontent.com/60553699/113494581-57941c00-949e-11eb-894b-0b7e54aed6c1.png">
