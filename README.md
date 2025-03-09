# BudgetFlow

## User Stories

# User Authentication & Security

- I want to securely sign up with an email and password so that my data is protected.
- I want to log in and log out securely so that my financial data remains private.

* I want to reset my password if I forget it so that I can regain access to my account.
* I want my session to persist using authentication tokens so that I don’t have to log in repeatedly.
  Calendar & Transaction Entry
* I want to view a monthly calendar where each day is represented as a clickable cell so that I can input financial transactions.
* I want to click on a date and enter an amount along with a description so that I can track my expenses and income.
* I want to enter multiple transactions per day so that I can track multiple expenses or sources of income.
* I want each transaction to be categorized as either a debit or credit so that I can track money flowing in and out.
* I want to see an indicator for days that have transactions so that I know where I have entered financial data.
  Transaction Journal & Running Totals
* I want a transaction journal displayed next to the calendar so that I can see all my transactions in one place.
* I want to see a running total of all debits and credits so that I can track my financial position.
* I want to mark a transaction as “posted” so that I can track what has already been deducted from my balance.
* I want to see a balance after deductions so that I can know my available funds after pending expenses.
  Navigation & User Experience
* I want to navigate between months so that I can plan ahead and review past transactions.
* I want the app to remember my last-viewed month so that I don’t have to navigate manually every time.
* I want a responsive design so that I can use the app on both desktop and mobile devices.
  Additional Features (Future Enhancements)
* I want to filter transactions by category so that I can analyze spending habits.
* I want to export my financial data to CSV so that I can back it up or analyze it in external tools.
* I want to set up recurring transactions so that I don’t have to enter fixed expenses manually each month.
* I want notifications/reminders for upcoming due payments so that I don’t miss any important expenses.

FRONTEND ROUTES
|Path | Purpose|
|-----| -------|
|`/` | Login page |
/signup Register page
/dashboard Overview of financial summary
/calendar Calendar view of transactions
/transactions View all transactions
/transactions/:id Detailed transaction view
/budget Set and manage budget goals
/reports Generate and view reports
/settings User settings and preferences

BACKEND ROUTES
Method Path Purpose
User Authentication
POST /api/v1/users/register Register a new user
POST /api/v1/users/login Log in a user
GET /api/v1/users/profile Fetch user profile details
PUT /api/v1/users/profile Update user profile details
Transactions
GET /api/v1/transactions Retrieve all user transactions
GET /api/v1/transactions/:id Retrieve a specific transaction
POST /api/v1/transactions Add a new transaction
PUT /api/v1/transactions/:id Edit a transaction
DELETE /api/v1/transactions/:id Delete a transaction
Budget & Financial Planning
GET /api/v1/budget Get budget goals
POST /api/v1/budget Set a new budget goal
PUT /api/v1/budget/:id Update a budget goal
DELETE /api/v1/budget/:id Delete a budget goal
Reports & Analysis
GET /api/v1/reports Fetch financial reports
POST /api/v1/reports/generate Generate a new report
Recurring Payments & Income
GET /api/v1/recurring Get all recurring payments
POST /api/v1/recurring Add a recurring payment
PUT /api/v1/recurring/:id Edit a recurring payment
DELETE /api/v1/recurring/:id Delete a recurring payment
