# Banking-Analysis-Power-BI-Dashboard

![Homepage](https://github.com/pkanphade/Banking-Analysis/assets/75200373/132a7131-e28d-48d2-9e33-67e83707340c)
![LoanAnalysis](https://github.com/pkanphade/Banking-Analysis/assets/75200373/417065cf-7b76-4621-ad2d-d410a95fae03)
![DepositAnalysis](https://github.com/pkanphade/Banking-Analysis/assets/75200373/013210a3-3361-4054-9667-86c1f2a17840)
![Summary](https://github.com/pkanphade/Banking-Analysis/assets/75200373/b0113584-954b-4487-b4f4-890dd7d2ee32)

## Introduction
The Banking Analysis Power BI Dashboard is a comprehensive tool designed to provide insights into various banking metrics. This dashboard is developed using four primary tables and several DAX queries to deliver a detailed analysis of banking relationships, client demographics, and financial metrics.

## Data Tables

 1. Banking Relationship

This table captures the core relationship between clients and their banking services.

- Columns

1. BRID: Banking Relationship ID
2. Banking Relationship: Type of banking relationship


###
 2. Clients - Banking

This table holds detailed information about clients and their banking contracts.

- Columns

1. Banking Contracts: Information on banking contracts
2. BRID: Banking Relationship ID (Foreign Key)
3. ClientID: Unique Identifier for clients
4. Fee Structure: Fee structure associated with the banking services
5. GenderID: Gender Identifier (Foreign Key)
6. IAID: Investment Advisor ID (Foreign Key)
7. Name: Client's name
8. Nationality: Client's nationality
9. Occupation: Client's occupation

###
 3. Gender

This table provides the gender details of clients.

- Columns

1. GenderID: Unique Identifier for gender
2. Gender: Gender Description

###
 4. Gender

This table contains information about investment advisors.

- Columns

1. IAID: Unique Identifier for investment advisors
2. Investment Advisor: Name of the investment advisor


## Key Metrics and DAX Queries

The dashboard includes several important metrics calculated using DAX queries to provide comprehensive insights:

Saving Account Amount

```bash
SavingAccountAmount = SUM('Clients - Banking'[Savings Accounts])
```

Total Credit Card Amount

```bash
TotalCCAmount = SUM('Clients - Banking'[Credit Card Balance])
```

Total Deposit

```bash
TotalDeposit = SUM('Clients - Banking'[Bank Deposits])
```

Total Loan

```bash
TotalLoan = SUM('Clients - Banking'[Bank Loans])
```
## Summation of Amounts

The following DAX queries calculate the summation of various financial accounts:

- Credit Cards
```bash
TotalCreditCards = SUM('Clients - Banking'[Credit Card Balance])
```
- Bank Deposits
```bash
TotalBankDeposits = SUM('Clients - Banking'[Bank Deposits])
```

- Bank Loans
```bash
TotalBankLoans = SUM('Clients - Banking'[Bank Loans])
```
- Business Lending
```bash
TotalBusinessLending = SUM('Clients - Banking'[Business Lending])
```

- Checking Accounts
```bash
TotalCheckingAccounts = SUM('Clients - Banking'[Checking Accounts])
```
- Credit Card Balance
```bash
TotalCreditCardBalance = SUM('Clients - Banking'[Credit Card Balance])
```

- Estimated Income
```bash
TotalEstimatedIncome = SUM('Clients - Banking'[Estimated Income])
```
- Foreign Currency Account
```bash
TotalForeignCurrencyAccount = SUM('Clients - Banking'[Foreign Currency Account])
```

- Savings Accounts
```bash
TotalSavingsAccounts = SUM('Clients - Banking'[Savings Accounts])
```
- Superannuation Savings
```bash
TotalSuperannuationSavings = SUM('Clients - Banking'[Superannuation Savings])
```

## Usage
The dashboard provides an intuitive interface to explore and analyze banking data. Users can filter data based on various parameters such as client demographics, banking relationships, and financial metrics. The visualizations include charts, graphs, and tables to offer a clear and concise representation of the data.

## Conclusion
The Banking Analysis Power BI Dashboard is a powerful tool for financial analysis and decision-making. By leveraging data from multiple sources and using DAX queries to calculate key metrics, it provides valuable insights into banking relationships, client demographics, and financial performance.

[Author](https://github.com/pkanphade)
