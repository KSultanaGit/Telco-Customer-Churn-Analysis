# TelcoCustomerChurnAnalysis
 Analyzing Customer Churn and generating Report Using Python and Power BI

## Datasource :

Dataset: Telco Customer Churn 

## Data Preparation:

Completed the Data transformation in python and performed complete Exploratory analysis . 
EDA Report: 

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


## Data Analysis (DAX):

Measures used in  all visualization are:

- Average MonthlyCharges = `AVERAGE('tel_churn'[MonthlyCharges])`

- Average TotalCharges = `AVERAGE('tel_churn'[TotalCharges])`

- churn count = `CALCULATE(COUNT('tel_churn'[Churn]), ALLSELECTED('tel_churn'[Churn]),'tel_churn'[Churn] = "Yes")`

- churn rate % = `DIVIDE(CALCULATE(COUNT('tel_churn'[Churn]), 'tel_churn'[Churn] = "yes" ), COUNT('tel_churn'[Churn]), 0)`

- Dependent in % = `DIVIDE(CALCULATE(COUNT('tel_churn'[Dependents]), 'tel_churn'[Dependents]="Yes",'tel_churn'[Churn]="Yes"), CALCULATE(COUNT('tel_churn'[Dependents]),'tel_churn'[Churn]="Yes"), 0)`

- Device protection in % = `DIVIDE(CALCULATE(COUNT('tel_churn'[DeviceProtection]), 'tel_churn'[DeviceProtection] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[DeviceProtection]),'tel_churn'[Churn]="Yes"),0)`

- Online backup in % = `DIVIDE(CALCULATE(COUNT('tel_churn'[OnlineBackup]), 'tel_churn'[OnlineBackup] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[OnlineBackup]),'tel_churn'[Churn]="Yes"),0)`

- Online security in % =`DIVIDE(CALCULATE(COUNT('tel_churn'[OnlineSecurity]), 'tel_churn'[OnlineSecurity] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[OnlineSecurity]),'tel_churn'[Churn]="Yes"),0)`

- Partner in % = `DIVIDE(CALCULATE(COUNT('tel_churn'[Partner]),'tel_churn'[Partner]="Yes",'tel_churn'[Churn]="Yes"), CALCULATE(COUNT('tel_churn'[Partner]), 'tel_churn'[Churn]="Yes"), 0)`

- Phone service in % =`DIVIDE(CALCULATE(COUNT('tel_churn'[PhoneService]), 'tel_churn'[PhoneService] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[PhoneService]),'tel_churn'[Churn]="Yes"),0)`

- SenioCitizen in % = `DIVIDE(CALCULATE(COUNT('tel_churn'[SeniorCitizen]),'tel_churn'[SeniorCitizen]=1,'tel_churn'[Churn]="Yes"), CALCULATE(COUNT('tel_churn'[SeniorCitizen]),'tel_churn'[Churn]="Yes"), 0)`

- Streaming Movies in % =`DIVIDE(CALCULATE(COUNT('tel_churn'[StreamingMovies]), 'tel_churn'[StreamingMovies] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[StreamingMovies]),'tel_churn'[Churn]="Yes"),0)`

- Streaming TV in % =`DIVIDE(CALCULATE(COUNT('tel_churn'[StreamingTV]), 'tel_churn'[StreamingTV] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[StreamingTV]),'tel_churn'[Churn]="Yes"),0)`

- Tech Support in % =`DIVIDE(CALCULATE(COUNT('tel_churn'[TechSupport]), 'tel_churn'[TechSupport] ="Yes", 'tel_churn'[Churn]="Yes"),CALCULATE(COUNT('tel_churn'[TechSupport]),'tel_churn'[Churn]="Yes"),0)`

## Data Visualization (Dashboard):

Data visualization for the data analysis (DAX) was done in Microsoft Power BI Desktop:

Dashboard: [View Dashboard](https://github.com/KSultanaGit/Telco-Customer-Churn-Analysis/blob/main/images/churn_dashboard.png)

## Insights:

As shown the data Visualization, It can be deduced that:

- Customers on the Two-Year contract, have been with the company for long, while most of the customers on Month-to-Month contract joined the company.
- The company is at risk of losing recently joined customers. based on the results from analysis.. if they decided to month-to-month contract.
- 7043 customers are at the risk of churn. and The churn rate is 27%  and yearly charges is $16.06M charges. and Monthly Charges is $456.12K monthly charges.
- 2955 tech tickets were opened and 3632 admin tickets were opened.
- Most of the churned customers  did not sign up for Online Security and tech support and  also did not sign up for Phone Services.
- It a lot of customers had an issue with Fiber Optic . Up to 42% of the customers churned were using Fiber Optic as their Internet Services.

## Recommendation:

- The Company could try convincing customers to subscribe to One-Year and Two-Year contract. The contract are not favorable to customers  as they tend to pay more monthly.
- Giving the discount to customers based on the some specific tasks is also good wat retaining them, specially those month-to-month contract.
- From analysis majority customers who churned did not sigh up for Online Security and Tech Support. These are the important services that customers should customers signup for. The company should educate customers  on the benefits of signing up for these services.
- Increase sale of 1 and 2 year contract by 5% each and Yearly increase of automatic payments by 5%.

---


Contributed by Khadija Sultana










