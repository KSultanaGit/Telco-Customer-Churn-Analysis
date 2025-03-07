# TelcoCustomerChurnAnalysis
 Analyzing Customer Churn and generating Report Using Python and Power BI

## Datasource :

Dataset: Telco Customer Churn 

## Data Preparation:

Completed the Data transformation in python and performed complete Exploratory analysis . 
EDA Report: [View EDA Report](https://github.com/KSultanaGit/Telco-Customer-Churn-Analysis/blob/main/Churn_Analysis_EDA_Report.pdf)

Then cleaned dataset was loaded into Microsoft Power BI Desktop for modeling and dashboard.

- `Customer churn dataset` which has `23 columns and 7043 rows` of observation

Data Cleaning for the dataset was done in the power query editor as follows:

- Replaced  the value is `SeniorCitizen` N coverted No and Y converted Yes

In the new table, one additional conditional columns were added such as tenure 
- Removed Unnecessary columns 
- Removed Unnecessary rows
- Each of the columns in the table were validated to have the correct data type

## Data Modeling:

And then dataset was cleaned and transformed, it was ready to the data modeled.


## Data Visualization (Dashboard):

Data visualization for the data analysis (DAX) was done in Microsoft Power BI Desktop.

<img src="https://github.com/KSultanaGit/Telco-Customer-Churn-Analysis/blob/main/images/churn_dashboard.png" alt="Screenshot 1" width="500" height="500" align="center">


## Insights:

As shown the data Visualization, It can be deduced that:

- Customers on the Two-Year contract, have been with the company for long, while most of the customers on Month-to-Month contract joined the company.
- The company is at risk of losing recently joined customers. based on the results from analysis.. if they decided to month-to-month contract.
- 7043 customers are at the risk of churn. and The churn rate is 27%  and yearly charges is $16.06M charges. and Monthly Charges is $456.12K monthly charges.
- Most of the churned customers  did not sign up for Online Security and tech support and  also did not sign up for Phone Services.
- It a lot of customers had an issue with Fiber Optic . 
- Up to 42% of the customers churned were using Fiber Optic as their Internet Services.

## Recommendation:

- The Company could try convincing customers to subscribe to One-Year and Two-Year contract. The contract are not favorable to customers  as they tend to pay more monthly.
- Giving the discount to customers based on the some specific tasks is also good wat retaining them, specially those month-to-month contract.
- From analysis majority customers who churned did not sigh up for Online Security and Tech Support. These are the important services that customers should customers signup for. The company should educate customers  on the benefits of signing up for these services.
- Increase sale of 1 and 2 year contract by 5% each and Yearly increase of automatic payments by 5%.

---


Contributed by Khadija Sultana










