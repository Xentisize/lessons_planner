# Lesson Planner for issuing invoices

Lesson planner is intended to save the trivial work from manually input the lessons for issuing invoices every month. Therefore, it should be able to accept input (dates, students, fees) from the user.

## Components

1. Database handler for interacting data
   - [ ] Student name
   - [ ] Default lesson's details (weekdays, duration, fees, teacher)
   - [ ] Proposed lessons
2. Module for working with date and calendar
   - [ ] construct a calendar for a month
   - [ ] search interchangeably between a date and a weekday
3. PDF output module
   - [ ] construct the layout
   - [ ] output in PDF format

## Proposed database tables

The database will be in sqlite3 for portability.  
Student ['First Name', 'Last Name', 'Full Name']  
=> has many  
Lesson ['Weekday', 'Duration', 'Fee', 'Subject', 'Teacher']  
=> has many  
Lesson Item ['Date', 'Duration', 'Fee']

Invoices
=> has many
Lesson -> PDF
