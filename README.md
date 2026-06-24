# Automated Email Campaign using n8n

## Overview

An automated email workflow built using **n8n**, **Google Sheets**, **Gmail**, and **JavaScript**.

The workflow reads user records from Google Sheets, selects the appropriate email template based on the user's type, personalizes the email by replacing placeholders, sends the email through Gmail, and updates the delivery status automatically.

## Features

* Read user data from Google Sheets
* Filter users whose emails have not been sent
* Match email templates based on User Type
* Personalize emails using `{{NAME}}` placeholders
* Send emails automatically through Gmail
* Update email delivery status in Google Sheets 
* Prevent duplicate email sending

## Workflow

```text
Google Sheets (Users)
        ↓
IF (Status != SENT)
        ↓
Loop Over Items
        ↓
Get Email Templates
        ↓
Personalize Content
        ↓
Gmail
        ↓
Update Status
```

## Technologies Used

* n8n
* Google Sheets
* Gmail
* JavaScript

## Sample Personalization

Template:

Hello {{NAME}}, welcome to our internship program.

Generated Email:

Hello Hemashree, welcome to our internship program.

## Future Improvements

* AI-generated email content
* Scheduled campaigns
* Analytics dashboard
* Multi-placeholder support

## Author

Hemashree S
