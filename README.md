# Personal Finance & Wealth Management System

A modern full-stack financial management platform that helps users track investments, loans, expenses, business funds, and overall financial health through automated calculations and analytics.

---

# Tech Stack

## Frontend

* Next.js 15
* TypeScript
* Tailwind CSS
* ShadCN UI
* React Hook Form
* Zod
* TanStack Query
* Axios
* Recharts

## Authentication

* Clerk Authentication
* Email/Password Login
* Google Login
* Email Verification
* Protected Routes

## Backend

* Node.js
* Express.js
* TypeScript
* Prisma ORM

## Database

* PostgreSQL
* Supabase PostgreSQL (Recommended)

---

# User Roles

The system contains only two roles.

## Admin

Admin can:

* Manage all users
* View all financial records
* Manage investments
* Manage loans
* Manage expenses
* Manage business funds
* Generate reports
* Export data
* Access analytics dashboard

---

## User

User can:

* Access personal dashboard
* Manage personal investments
* Manage personal loans
* Manage personal expenses
* View personal reports
* View financial analytics

User cannot:

* Access other users' data
* Manage users
* View admin-only analytics

---

# Core Features

## Authentication

### Registration

Users can:

* Create an account
* Verify email
* Login securely
* Logout
* Reset password

### Login

Supported methods:

* Email & Password
* Google Authentication

---

# Financial Modules

## Investment Management

Track:

* Investment Type
* Platform
* Amount
* Current Value
* Profit/Loss
* Notes

### Automatic Calculation

ROI = ((Current Value - Investment Cost) / Investment Cost) × 100

---

## Loan Management

### Loan Taken

Track:

* Creditor Name
* Loan Amount
* Due Date
* Paid Amount
* Remaining Balance

### Loan Given

Track:

* Borrower Name
* Loan Amount
* Return Date
* Collection Status

### Automatic Calculation

Outstanding Balance = Total Loan - Paid Amount

---

## Expense Management

Categories:

* Food
* Transport
* Rent
* Shopping
* Education
* Healthcare
* Utilities
* Others

Track:

* Amount
* Category
* Date
* Notes

---

## Business Fund Management

Track:

* Fund Name
* Partners
* Contributions
* Revenue
* Expenses
* Profit Distribution

### Profit Sharing Formula

Partner Share = Total Profit × Ownership Percentage

---

# Automated Financial Calculations

Users only enter data.

All financial metrics are automatically calculated in the background.

---

## Total Assets

Total Assets =
Cash +
Bank Balance +
Investments +
Loans Receivable +
Business Equity

---

## Total Liabilities

Total Liabilities =
Loans Payable +
Outstanding Debts

---

## Net Worth

Net Worth =
Total Assets -
Total Liabilities

---

## Cash Flow

Cash Flow =
Income -
Expenses

---

## Savings Rate

Savings Rate =
(Savings / Income) × 100

---

## Debt Ratio

Debt Ratio =
(Liabilities / Assets) × 100

---

## Investment ROI

ROI =
((Current Value - Investment Cost) / Investment Cost) × 100

---

## Profit Margin

Profit Margin =
(Net Profit / Revenue) × 100

---

## Financial Health Score

Financial Health Score =
(40% Net Worth Score)
+
(30% Savings Score)
+
(20% Debt Score)
+
(10% Cash Flow Score)

### Score Levels

| Score  | Status    |
| ------ | --------- |
| 0-40   | Poor      |
| 41-60  | Average   |
| 61-80  | Good      |
| 81-100 | Excellent |

---

# Dashboard

The dashboard displays:

* Net Worth
* Total Assets
* Total Liabilities
* Cash Flow
* Savings Rate
* Debt Ratio
* Investment ROI
* Business Profit
* Outstanding Loans
* Financial Health Score

---

# Reports

Generate:

* Monthly Reports
* Yearly Reports
* Investment Reports
* Loan Reports
* Expense Reports
* Business Reports

---

# Export Features

Supported Formats:

* Excel (.xlsx)
* CSV
* PDF

---

# Project Structure

```bash
personal-finance-system/
│
├── frontend/
├── backend/
├── docs/
├── README.md
└── .gitignore
```

---

# Frontend Structure

```bash
frontend/
│
├── public/
│
├── src/
│
├── app/
│   ├── (auth)/
│   │   ├── sign-in/
│   │   ├── sign-up/
│   │   └── verify/
│   │
│   ├── dashboard/
│   ├── investments/
│   ├── loans/
│   ├── expenses/
│   ├── funds/
│   ├── reports/
│   └── settings/
│
├── components/
│   ├── ui/
│   ├── shared/
│   ├── forms/
│   ├── charts/
│   └── tables/
│
├── hooks/
├── services/
├── store/
├── lib/
├── types/
├── utils/
│
├── middleware.ts
└── package.json
```

---

# Backend Structure

```bash
backend/
│
├── src/
│
├── config/
├── middleware/
├── routes/
├── controllers/
├── services/
├── repositories/
├── validations/
├── utils/
│
├── modules/
│   ├── users/
│   ├── investments/
│   ├── loans/
│   ├── expenses/
│   ├── funds/
│   ├── analytics/
│   └── reports/
│
├── app.ts
├── server.ts
│
├── prisma/
│   ├── schema.prisma
│   └── migrations/
│
└── package.json
```

---

# Database Tables

```text
users
investments
loans_taken
loans_given
expenses
funds
fund_members
businesses
business_transactions
reports
```

---

# Security Features

* Clerk Authentication
* Protected Routes
* Role-Based Access Control
* Password Security Managed by Clerk
* Secure API Access
* Server-side Validation
* Zod Validation
* Input Sanitization

---

# Future Enhancements

* AI Financial Advisor
* Expense Prediction
* Investment Forecasting
* Mobile App
* Push Notifications
* Multi-Currency Support
* Bank API Integration
* OCR Receipt Scanning
* AI Budget Planning

---

# Development Principles

* Clean Architecture
* SOLID Principles
* Feature-Based Folder Structure
* Reusable Components
* Type Safety
* Scalable Design
* Maintainable Codebase

---

# Project Objective

Build a modern, secure, scalable, and user-friendly Personal Finance & Wealth Management Platform that enables users to manage assets, liabilities, investments, loans, expenses, and business finances through automated financial calculations and real-time analytics.
