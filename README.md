# finOX---Python-Based-Desktop-Application
Python-based desktop application for personal and family financial management. Supports personalized budgeting, income and expense tracking, savings, debt and loan management, financial goals, family &amp; individual budgets, database storage, charts, reports, and future AI/ML-based forecasting.


# Project Description

**finOX** is a Python-based desktop application designed for personalized personal and family financial planning and management. The system combines a graphical user interface (GUI), database-based storage, automated calculation, expense tracking, budgeting, savings management, financial goals, visualization, and reporting.

Unlike a simple one-size-fits-all budgeting application, finOX considers **family composition, member age, number of members, individual and household income, district/area, cost-of-living data, priorities, recurring expenses, savings goals, and other financial requirements** to generate a personalized financial plan.

---

## 🔄 Overall Working Process

The complete finOX workflow follows these major steps:

### 1. Account Registration & Sign In

The user first creates an account through **Sign Up** and then accesses the system through **Sign In**.

The account system manages:

* User profile
* Family information
* Financial information
* Access permissions
* Individual and shared family financial management

---

### 2. Create User Profile

The user provides basic information such as:

* Name
* District / Area
* Family category
* Monthly income
* Occupation
* Other relevant profile information

The district/area is stored in the database and later connected with area-specific cost-of-living and market data.

---

### 3. Select Family Category

The user selects a general family category:

* Single Person
* Couple
* Family
* Custom Family Type

The system is not restricted to a fixed family size or fixed number of members.

---

### 4. Add Family Members

The user can add family members individually.

For each member, finOX stores:

* Name
* Age
* Gender
* Relation
* Income status
* Monthly income
* Dependent / Non-dependent status

The system supports children, parents, grandparents, siblings, multiple generations, and other household members.

---

### 5. Determine Age-Based Requirements

Based on the member's age, finOX identifies the relevant age group, such as:

* Infant / Toddler
* Child
* Teenager
* Adult
* Senior

Age-based requirements can influence areas such as **food, nutrition, healthcare, education, and other household expenses**.

---

### 6. Add Individual Income

Income is recorded separately for each earning member.

Possible income sources include:

* Salary
* Freelancing
* Business
* Part-time work
* Other income

The system then calculates:

**Total Household Income = Sum of All Earning Members' Income**

For multiple earners, finOX can also calculate individual contribution, shared contribution, individual remaining amount, and individual savings.

---

### 7. Enter District / Area

The user enters their district and area.

finOX retrieves the relevant information from the **database**, including:

* Housing / Rent
* Food
* Transportation
* Utilities
* Healthcare
* Education
* Other essential costs

The system uses these data to determine the area's **Low / Medium / High cost-of-living level**.

The cost-of-living level is therefore **data-driven**, rather than simply assigning a fixed level to a district.

---

### 8. Enter Expenses & Financial Information

Users can enter their existing or expected expenses.

Expense categories may include:

* Food & Nutrition
* Housing / Rent
* Utilities
* Transportation
* Education
* Healthcare
* Personal Expenses
* Family Expenses
* Entertainment
* Savings
* Debt / Loan
* Emergency Fund
* Investment
* Custom Expenses

Recurring expenses such as rent, utilities, subscriptions, and loan EMI can also be stored.

---

# 🧮 9. Database-Driven Budget Calculation

This is one of the core features of finOX.

The **percentage allocation is not simply hard-coded inside the Python program**.

Instead, finOX stores budget-related information in the database, such as:

* Budget rules
* Category information
* Category percentages
* Priority weights
* Area-specific cost data
* Market prices
* Family/age-related rules
* Savings targets
* Other calculation-related data

The Python **Calculation Engine** retrieves the required information from the database and combines it with the user's current financial information.

### Basic Calculation

The system can use:

**Allocated Amount = Available Income × Category Percentage / 100**

For example, if the database provides a percentage for a specific category, the Calculation Engine retrieves that percentage and calculates the allocated amount based on the user's available income.

Therefore:

**Database → Budget Rules / Percentage → Python Calculation Engine → Personalized Allocation**

The percentage can be adjusted according to:

* Family structure
* Number of members
* Age groups
* District / Area
* Cost-of-living conditions
* User priorities
* Fixed expenses
* Recurring expenses
* Savings goals
* Market prices
* Other financial requirements

This makes the budgeting system **dynamic and database-driven**.

---

## 10. Select Budgeting Method

finOX supports multiple budgeting mechanisms.

### Percentage-Based Budgeting

Income is distributed among categories using percentages stored in the database.

Possible categories include:

* Needs
* Wants
* Savings
* Debt Repayment

The database provides the required percentage/rules, and the Python engine performs the calculation.

### Zero-Based Budgeting

Every part of the available income is assigned a purpose.

Income can be allocated to:

* Expenses
* Savings
* Investments
* Debt repayment

### Envelope-Based Budgeting

Available money is divided into digital spending categories or "envelopes."

Examples:

* Food
* Transportation
* Education
* Entertainment

The system can use income, priorities, expenses, and database-stored rules to determine the allocation.

---

## 11. Apply Priority-Based Planning

Users can assign priorities such as:

* **Essential**
* **Important**
* **Optional**

Fixed and recurring expenses such as rent, utilities, and loan EMI can be considered first.

The remaining available income is then allocated among other categories and savings according to priorities and database-driven rules.

---

## 12. Generate Personalized Budget

After processing all relevant information, the Calculation Engine generates:

* Category-wise allocated amount
* Total allocated amount
* Expected spending
* Available amount
* Savings amount
* Savings rate
* Family budget
* Individual budget for account-holding members

The budget can be recalculated whenever important information changes.

For example:

**Income Change → Recalculate Budget**

**Family Member Added → Recalculate Budget**

**Expense Change → Recalculate Budget**

**Market Price Change → Recalculate Budget**

**Savings Goal Change → Recalculate Budget**

---

## 13. Track Daily Expenses

Users record daily spending with information such as:

* Date
* Time
* Category
* Amount
* Description
* Location / Source
* Payment Method
* Family Member
* Shared / Individual Expense

finOX continuously updates:

**Allocated → Already Spent → Available**

If spending exceeds the available budget, the system can provide a warning.

---

## 14. Manage Savings

finOX manages both **family savings and individual savings**.

The system can calculate:

* Total family savings
* Individual savings
* Monthly savings
* Savings rate
* Savings target
* Required monthly savings
* Progress toward savings goals

---

## 15. Manage Emergency Fund

Users can create a separate emergency fund.

The system can:

* Track current emergency savings
* Calculate required emergency savings
* Suggest regular savings
* Estimate how many months of expenses the fund can cover

---

## 16. Manage Debt & Loans

finOX can manage:

* Loans
* Debt
* EMI
* Repayment timeline
* Remaining amount
* Repayment history
* Lending
* Borrowing

Repayment planning can consider loan amount, income, interest details, and monthly repayment amount.

---

## 17. Set Financial Goals

Users can create financial goals such as:

* Investment
* Marriage
* Overseas Education
* Emergency Fund
* Entertainment
* Major Life Events

For each goal, the system can calculate:

**Target Amount → Current Savings → Target Date → Required Monthly Savings → Progress**

---

## 18. Family & Individual Budget Management

finOX supports both:

### Family Budget

Shared:

* Income
* Expenses
* Savings
* Budget
* Financial goals

### Individual Budget

Each account-holding family member can separately manage:

* Individual income
* Individual expenses
* Individual savings
* Individual priorities
* Personal financial goals

Therefore, finOX connects:

**Individual Financial Management ↔ Shared Family Financial Management**

---

## 19. Store Everything in Database

The database stores structured financial information including:

* Users
* Family members
* Family relationships
* Income
* Expenses
* Budget plans
* Budget allocations
* Budget rules
* Category percentages
* Savings
* Financial goals
* Emergency funds
* Loans
* Investments
* Monthly history
* District / Area data
* Cost-of-living data
* Market prices
* Notifications

The database allows finOX to retrieve information, update records, recalculate budgets, maintain history, and generate reports.

---

## 20. Monthly History

At the end of each period, finOX can maintain historical financial records including:

* Income
* Expenses
* Budget allocations
* Savings
* Family information
* Cost-of-living level
* Monthly financial summary

Historical data can later be used for trend analysis and forecasting.

---

## 21. Visualization & Reports

finOX provides graphical visualization of:

* Income
* Expenses
* Savings
* Investments
* Category-wise spending
* Monthly spending
* Budget vs Actual Spending
* Financial Goal Progress

The system can also generate financial reports such as:

* Income Report
* Expense Report
* Savings Report
* Budget Report
* Investment Report
* Debt Report
* Monthly Financial Summary
* Family Financial Summary

---

## 22. Notifications & Alerts

The system can notify users about:

* Budget limits
* Spending limits
* Bill payments
* Recurring expenses
* Savings targets
* Financial goals

It can also provide suggestions when spending patterns indicate that the budget may need adjustment.

---

## 23. Future AI/ML Features

Historical financial data can later support AI/ML-based features such as:

* Expense forecasting
* Smart expense categorization
* Financial recommendations
* What-if scenario analysis
* Spending pattern analysis

Example scenarios:

* What if income decreases?
* What if income increases?
* What if prices increase?
* What if a new family member is added?
* What if a major expense occurs?

---

# 🏗️ System Architecture

The overall architecture of finOX follows:

**User / Family Data**
↓
**Family Member Profiles**
↓
**Optional Individual Accounts**
↓
**Sign Up / Sign In**
↓
**Access Permissions**
↓
**Database**
↓
**Area Data / Market Data / Budget Rules / Historical Data**
↓
**Python Calculation Engine**
↓
**Family Budget + Individual Budget**
↓
**Expense Tracking / Savings / Goals / Debt / Investment**
↓
**Charts / Reports / Notifications**
↓
**Historical Analysis / Forecasting / AI-ML**

---

# 🛠️ Technology

* **Python**
* **Desktop GUI**
* **Database Management System**
* **Python-based Calculation Engine**
* **Data Visualization**
* **Reporting System**
* **Future AI/ML Integration**

---

# 🎯 Project Goal

The main goal of finOX is to provide a **personalized, family-aware, and database-driven financial planning system** instead of relying on a generic one-size-fits-all budget.

The system uses:

**User Data + Family Data + Age + Income + Area Data + Cost of Living + Market Data + Priorities + Database Rules**

to generate:

**Personalized Budget → Expense Tracking → Savings Planning → Financial Goals → Reports & Analysis**

The key concept is that **budget rules and percentage allocations are stored in the database, while the Python Calculation Engine retrieves and applies those rules dynamically** according to the user's financial situation.
