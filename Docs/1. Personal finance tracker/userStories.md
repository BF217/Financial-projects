# Personal finance tracker - Epics and User Stories

---

# Epics

1. User Authentication and Authorisation
2. Transactional Management
3. Financial Reporting
4. Dashboard Overview
5. User Notifications
6. Settings and Preferences

---

# Epic 1: User Authentication and Authorisation

---

## User Stories

---

## 1. User registration

---

### Priority: High

### User: new user who wants to sign up for our services

### User Story:

As a new user, I want to create an account, so that I can access the personal finance tracker.

### Tasks:

#### Frontend:

- Create a registration form with fields for email, password, and confirmation password. Possibly use external sign up options.
- Validate user inputs (e.g. email format, password strength).
- Integrate with backend API for user registration.

#### Backend:

- Set up endpoint for user registration.
- Implement validation logic.
- Store data in MongoDB.
- Handle error responses (e.g. user already exists).

### Acceptance criteria:

- User can register with a valid email and password.
- User receives error messages for invalid inputs.
- User data is stored in the database.

---

## 2. User Login

---

### Priority: High

### User: A registered user

### User Story:

as a registered user, I want to log in to my account, so that I can access my financial data.

### Tasks:

#### Frontend:

- Create a login form with fields for email and password.
- Validate user inputs
- Integrate with backend API for user authentication.

#### Backend:

- Set up endpoint for user login.
- Validate credentials against the database.
- Implement JWT token generation for session management.

### Acceptance Criteria:

- User can log in with valid credentials.
- User receives an error message for invalid credentials.
- User session is managed using JWT tokens.

---

## 3. Password Recovery

---

### Priority: Medium

### User: Someone who has forgotten their password

### User Story

As a user who has forgotten my password, I want to reset my password so that I can regain access to my account.

### Tasks:

#### Frontend:

- Create a password recovery form with an email field.
- Integrate with backend API to request a password reset.

#### Backend:

- Set up endpoint for password recovery.
- Implement email service to send password reset link.
- Handle password reset logic.

### Acceptance Criteria:

- User can request a password reset with a valid email.
- User receives a password reset email.
- User can reset the password using the provided link.

---

# Epic 2: Transaction Management

---

## 4. Add Transaction

---

### Priority: High

### User: Signed in user

### User Story

As a user, I want to add a new financial transaction, so that I can track my income and expenses.

### Tasks:

#### Frontend:

- Create a form for adding transactions with fields for amount, date, category, and description.
- Validate user inputs.
- Integrate with backend API to save the transaction.

#### Backend:

- Set up endpoint for adding transactions.
- Implement logic to save transaction data in MongoDB.
- Handle validation and error responses.

### Acceptance Criteria:

- User can add a transaction with valid inputs.
- Transaction data is stored in the database.
- User receives confirmation upon successful addition.

---

## 5. Edit Transaction

---

### Priority: Medium

### User: Signed in user

### User Story

As a user, I want to edit an existing transaction, so that I can correct any mistakes or update details.

### Tasks:

#### Frontend:

- Create a form for editing transactions pre-filled with existing data.
- Validate user inputs.
- Integrate with backend API to update the transaction.

#### Backend:

- Set up endpoint for editing transactions.
- Implement logic to update transaction data in MongoDB.
- Handle validation and error responses.

### Acceptance Criteria:

- User can edit a transaction with valid inputs.
- Updated transaction data is stored in the database.
- User receives confirmation upon successful update.

---

## 6. Delete Transaction

---

### Priority: Medium

### User: Signed in user

### User Story

As a user, I want to delete a transaction, so that I can remove any incorrect or unwanted entries.

### Tasks:

#### Frontend:

- Implement a delete button for transactions.
- Integrate with backend API to delete the transaction.

#### Backend:

- Set up endpoint for deleting transactions.
- Implement logic to remove transaction data from MongoDB.

### Acceptance Criteria:

- User can delete a transaction.
- Transaction data is removed from the database.
- User receives confirmation upon successful deletion.

---

# Epic 3: Financial Reporting

---

## 7. view Monthly Report

---

### Priority: High

### User: signed in user

### User Story

As a user, I want to view a report of my monthly income and expenses, so that I can understand my financial status.

### Tasks:

#### Frontend:

- Create a page to display the monthly report.
- Integrate with backend API to fetch monthly transaction data.
- Implement charts and summaries to visualise the data.

#### Backend:

- Set up endpoint to fetch monthly transactions.
- Implement logic to aggregate data by month.

### Acceptance Criteria:

- User can view a detailed monthly report.
- report includes charts and summaries.
- Data is accurate and up to date.

---

## 8. Generate Custom Reports

---

### Priority: Low

### User:

### User Story

As a user, I want to generate custom financial reports based on specific criteria, so that I can analyse my finances.

### Tasks:

#### Frontend:

- Create a form for selecting report criteria (e.g. data range, categories)
- Integrate with backend API to fetch custom data report.

#### Backend:

- Set up endpoint to fetch custom report data.
- Implement logic filter and aggregate data based on criteria.

### Acceptance Criteria:

- User can generate reports based on selected criteria.
- Report includes detailed breakdown and visualisations.
- Data is accurate and meets user-selected criteria.

---

# Epic 4: Dashboard Overview

---

## 9. Dashboard Summary

---

### Priority: High

### User:

### User Story

As a user, I want to view a summary of my financial status on the dashboard, so that I can quickly understand my overall finances.

### Tasks:

#### Frontend:

- Create a dashboard page with summary widgets (e.g. total income, total expenses, net balance).
- Integrate with backend API to fetch summary data.

#### Backend:

- Set up endpoint to fetch summary data.
- Implement logic to calculate and aggregate summary information.

### Acceptance Criteria:

- User can view a dashboard with financial summaries.
- Data is accurate and updated in real-time.
- Dashboard includes interactive elements for detailed views.

---

# Epic 5: User Notifications

---

## 10. Transaction Notifications

---

### Priority: Medium

### User:

### User Story

As a user, I want to receive notifications for important transaction activities, so that I can stay informed about my finances.

### Tasks:

#### Frontend:

- Implement notification system for transaction activities (e.g. addition, deletion).
- integrate with backend API to receive notification data.

#### Backend:

- Set up notification system for transaction activities.
- implement logic to trigger notifications based on transaction activities.

### Acceptance Criteria:

- User receives notifications for transaction activities.
- Notifications are clear and actionable.
- User can manage notification preferences.

---

# Epic 6: Settings and Preferences

---

## 11. Manage User Profile

---

### Priority: Medium

### User:

### User Story

As a user, I want to update my profile information, so that I can keep my account details up to date.

### Tasks:

#### Frontend:

- Create a profile page with fields for updating user information.
- Integrate with backend API to save profile changes.

#### Backend:

- Set up endpoint for updating user profile.
- Implement logic to save profile changes in MongoDB.

### Acceptance Criteria:

- User can update profile information.
- Changes are saved and reflected in the database.
- User receives confirmation upon successful update.

---

## 12. Notification Preferences

---

### Priority: Medium

### User:

### User Story

As a user, I want to manage my notification preferences, so that I can control the types of notifications I receive.

### Tasks:

#### Frontend:

- Create a notification settings page with options to enable/disable notifications.
- Integrate with backend API to save notification preferences.

#### Backend:

- Set up endpoint for managing notification preferences.
- Implement logic to save user preferences in MongoDB.

### Acceptance Criteria:

- User can set and update notification preferences.
- Preferences are saved and applied to notification system.
- User receives confirmation upon successful update.

---
