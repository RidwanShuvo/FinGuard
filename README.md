# FinGuard: Personal Finance Dashboard

## 📖 Overview
**FinGuard** is a personal finance dashboard which basically keeps track about your financial things like incomes,expenditures and other financial goals.It empowers users to control their finances.FinGuard categorizes the balance sheet according to incomes,expenses etc. which is easy to understand the finance dashboard.

---

##📝Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Software Development Life Cycle Phases](#sdlc-phases)
   - [Planning](#planning)
   - [Requirements Gathering & Analysis](#requirements-gathering-and-analysis)
   - [Design](#design)
   - [Implementation](#implementation)
   - [Testing](#testing)
   - [Deployment](#deployment)
   - [Maintenance](#maintenance)
5. [Project Timeline](#project-timeline)
6. [Challenges and Solutions](#challenges-and-solutions)
7. [Conclusion](#conclusion)

---
## Introduction
**FinGuard** is built to provide users with an easy way to manage their personal finances. It consolidates all financial data in one place, helping users make informed decisions about their spending habits and savings and we can easily know what amount of moneys are available.

---

## Features
- *Dashboard View*: Displays summary of income, expenses, and balance.
- *Expense Tracker*: Track and categorize expenses.
- *Budget Planning*: Set monthly budgets for different categories.
- *Investment Overview*: Track your investments and returns.
- *Financial Insights*: View spending patterns and identify savings opportunities.
- *Secure Data Storage*: Data is encrypted for privacy and security.

---

## Technologies Used
- *Frontend*: React.js, HTML, CSS
- *Backend*: Node.js, Express
- *Database*: MongoDB

---
## 🔄 Software Development Life Cycle (SDLC)

### 1. **Planning**
- **Objective**: To create a platform that consolidates financial data, enabling users to monitor their spending and achieve financial goals.
- **Scope**:
  - Track expenses and income.
  - Provide insights through reports and charts.
  - Allow users to set financial goals and monitor progress.
- **Stakeholders**: End-users, developers, project manager, finance advisors.
- **Risks**:
  - Data privacy concerns.
  - Complexity of third-party bank API integration.

---

### 2. **Requirements Gathering & Analysis**
- **Functional Requirements**:
  - User registration and login.
  - Track and categorize transactions.
  - Generate financial reports (PDF/CSV).
  - Set and monitor financial goals.
- **Non-Functional Requirements**:
  - Data encryption for security.
  - Scalable and fast-loading platform.
- **Tools & Technologies**:
  - Backend: Node.js/Django.
  - Frontend: React/Angular.
  - Database: PostgreSQL/MongoDB.
  - APIs: Plaid/Yodlee for bank integration.

---

### 3. **Design**
- **System Architecture**:
  - **Frontend**: Single Page Application (SPA) using React.
  - **Backend**: RESTful APIs with Node.js.
  - **Database**: Relational database (PostgreSQL).
- **UI/UX Design**:
  - Wireframes and prototypes in Figma.
  - Responsive and intuitive interface for web and mobile.
- **Database Schema**:
  - Users: `UserID, Name, Email, Password`
  - Transactions: `TransactionID, UserID, Amount, Category, Date`
  - Goals: `GoalID, UserID, GoalName, TargetAmount, Progress`
- **Security**:
  - Password hashing with bcrypt.
  - Two-Factor Authentication (2FA).
  - TLS encryption for secure communication.

---

### 4. **Development**
- **Frontend Development**:
  - Build the user interface with React.
  - Create reusable components for charts, tables, and forms.
- **Backend Development**:
  - Develop APIs for user authentication, transaction management, and goal tracking.
  - Implement third-party bank API integration.
- **Version Control**:
  - Git for source code management.
  - CI/CD pipelines using GitHub Actions.
- **Setup**:
  - Local development with Docker for consistent environments.
  - Linter and formatter tools (ESLint, Prettier).

---

### 5. **Testing**
- **Unit Testing**: Validate individual functions and components using Jest/Mocha.
- **Integration Testing**: Test data flow between frontend and backend.
- **User Acceptance Testing (UAT)**: Gather feedback from real users to ensure usability.
- **Security Testing**: Perform penetration tests to identify vulnerabilities.
- **Performance Testing**: Stress test to ensure scalability and responsiveness.

---

### 6. **Deployment**
- **Staging Deployment**:
  - Host a staging environment on AWS for final testing.
- **Production Deployment**:
  - Deploy on cloud platforms like AWS/Azure.
  - Set up monitoring tools (CloudWatch, New Relic).
- **Access**:
  - Staging: `http://staging.finguard.com`
  - Production: `http://www.finguard.com`

---

### 7. **Maintenance**
- Regular updates to fix bugs and add new features.
- Ongoing monitoring for performance and security.
- Periodic backups of user data.

---

## Project Timeline
| *Phase*         | *Start Date*  | *End Date*    |
|-------------------|-----------------|-----------------|
| Planning          | January 2024    | February 2024   |
| Design            | February 2024   | March 2024      |
| Implementation    | March 2024      | June 2024       |
| Testing           | June 2024       | July 2024       |
| Deployment        | July 2024       | August 2024     |
| Maintenance       | Ongoing         | Ongoing         |

---

## Challenges and Solutions
- *Challenge 1*: Integrating the expense categorization feature with third-party APIs.
  - *Solution*: We implemented a custom API to handle expense categorization, and we used pre-existing libraries to simplify integration with external services.
  
- *Challenge 2*: Ensuring data security for sensitive financial information.
  - *Solution*: We implemented end-to-end encryption for all sensitive data and used JWT for secure authentication.
---

## Conclusion
*FinGuard* provides a user-friendly, secure, and feature-rich platform to manage personal finances. With a clear development path through the SDLC phases, we ensured the application meets the needs of users while maintaining a high level of security and performance.

We plan to continue improving the dashboard based on user feedback and technological advancements.

---
