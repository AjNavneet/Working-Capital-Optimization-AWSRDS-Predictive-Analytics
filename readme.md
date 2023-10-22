# Working Capital Optimization using Predictive Analytics

## Project Overview

Working capital optimization involves strategically managing a company's current assets and liabilities to enhance operational efficiency and financial health. It focuses on finding the right balance between accounts receivable (AR) and accounts payable (AP) to ensure sufficient liquidity while minimizing costs and risks.

In this project, the aim is to predict the timing of customer payments and supplier payments through predictive modeling. By analyzing historical data, the project helps forecast the weeks when customers are likely to pay the company and when the company should pay its suppliers. These predictions enable proactive cash flow management, ensuring that customer payments cover outgoing payments to suppliers.

---

### Aim
The project's goal is to optimize working capital management by leveraging accounts receivable and payable data. Predictive analysis is used to accurately forecast the timing of customer and supplier payments, enabling the company to ensure cash flow and liquidity within a specified period.

---

### Data Description

#### Customer Data:
- Customer ID: Unique customer identifier.
- Customer Name: Customer's name.
- Customer Payment Terms: Payment terms and conditions for customers.
- Address: Physical address or location of the customer.
- Credit Limit: Maximum credit amount extended to the customer.

#### Receivables Data:
- Business Code: Code representing the type of business transaction.
- Customer Number: Unique customer identifier.
- Customer Name: Customer's name.
- Payment Date: Date of payment received.
- Business Year: Year of the business transaction.
- Posting Date: Date of posting the transaction.
- Due Date: Date by which the payment is due.
- Payterm: Payment terms for the invoice.
- Invoice Currency: Currency in which the invoice is issued.
- Total Open Amount: Total amount of the invoice.
- USD Currency: Currency conversion rate to USD.
- Total Open Amount (USD): Total amount in USD.
- Invoice ID: Unique identifier for each invoice.
- Is Open: Indicates whether the invoice is open or closed.
- DUNNLEVEL: Dunn level of the invoice, representing the past-due status.
- Credit Limit: Credit limit assigned to the customer.
- Baseline Date: Baseline date for the transaction.
- Region: Geographic region associated with the transaction.

#### Suppliers Data:
- Supplier ID: Unique supplier identifier.
- Supplier Name: Supplier's name.
- Payment Terms: Terms and conditions for supplier payments.
- Vendor Type: Type or category of the vendor/supplier.
- Supplier Category: Categorization of the supplier.

#### Payables Data:
- Invoice Number: Unique identifier for each invoice.
- Posting Date: Date of posting the invoice.
- Invoice Date: Date of the invoice.
- Payment Date: Date of payment made.
- Net Due Date (System Calculated Date): Calculated date for net payment due.
- Supplier ID: Unique supplier identifier.
- Invoice Amount: Total amount of the invoice.
- Fiscal Year: Financial year associated with the invoice.
- Overdue: Indicates if the payment is overdue.
- Invoice Status: Status of the invoice (e.g., paid, outstanding).
- Spend Category: Categorization of the expenditure.
- Total Outstanding Amount: Total amount outstanding for the invoice.
- Late Payment Fees: Fees charged for late payments.
- Payterm_n: Payment terms for the invoice.
- Vendor Type: Type or category of the vendor/supplier.

---

### Tech Stack
- Language: `Python`
- Libraries: `pandas`, `numpy`, `matplotlib`, `statsmodels`, `seaborn`, `scikit-learn`, `pyodbc`

---

## Approach

#### AR Data:
- Exploratory Data Analysis (EDA): Analyze accounts receivable data to gain insights into the distribution, trends, and patterns.
- Feature Engineering: Transform and manipulate AR data to extract relevant features for the prediction model.
- Model Building: Utilize various regression models (RandomForestRegressor, LinearRegression, KNeighborsRegressor, GradientBoostingRegressor, and SVR) to predict the week of customer payments.

#### AP Data:
- EDA: Perform exploratory analysis on accounts payable data to understand its characteristics and identify anomalies.
- Feature Engineering: Engineer additional features from the AP data that may be relevant for the analysis and prediction.
- Model Building: Develop prediction models based on the AP data to forecast the week of supplier payments.

#### Working Capital Optimization (WCO) Calculations:
- Group and sum receivables and payables data on a weekly basis.
- Calculate working capital by subtracting the sum of payables from the sum of receivables for each week.
- Analyze working capital figures to identify periods of positive or negative cash flow and assess overall liquidity.

---

## Concepts Explored

- Exploratory data analysis of accounts receivable and payable data.
- Transforming and manipulating for financial predictive modeling.
- Build regression models using various algorithms such as RandomForestRegressor, LinearRegressor, KNeighborsRegressor, GradientBoostingRegressor, and SVR.
- Importance of different features in predicting payment timings.
- Predicting and forecasting cash flow based on customer payments and supplier payments.
- Optimize working capital by analyzing and managing the balance between accounts receivable and payable.
- Communicate the results and insights derived from the predictive models.
- Applying data analysis and predictive modeling techniques to real-world financial data.
- Financial concepts, working capital management, and their impact on business performance.

---