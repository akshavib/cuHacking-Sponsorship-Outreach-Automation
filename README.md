cuHacking Sponsorship Outreach Automation
This project automates sponsorship outreach by integrating Google Sheets and Gmail using Google Apps Script. It helps streamline email communication for sponsorships, including drafting and sending personalized emails based on spreadsheet data.

Features
Automated Email Sending/Drafting: Automatically sends or drafts personalized emails for each sponsor listed in a Google Sheet.
Dynamic Email Templates: Fetches and customizes email templates from Google Docs, replacing placeholders (e.g., [FIRST_NAME], [COMPANY_NAME], etc.) with real values from the spreadsheet.
Column Header Mapping: Dynamically identifies relevant data (e.g., company name, representative's name, email address) by detecting headers in the Google Sheet.
Seamless Integration: Connects Google Sheets and Gmail for efficient outreach, minimizing manual work.
Setup Instructions
Prerequisites
A Google Account with access to Google Sheets and Google Docs.
A Google Sheet with sponsor data. The sheet should include headers such as:
Company Name
Rep. Full Name
Role
Email Address
cuHacking Correspondent
Google Apps Script access.
Steps
Clone this repository:

bash
Copy code
git clone https://github.com/akshavib/cuHackingSponsorshipOutreachAutomation.git
Set up the Google Sheet:

Update the Google Sheet with sponsorship data.
Ensure the headers in the sheet match the ones used in the code: Company Name, Rep. Full Name, Role, Email Address, and cuHacking Correspondent.
Set up Google Apps Script:

In the Google Sheet, go to Extensions > Apps Script.
Copy and paste the code from cuHackingSponsorshipOutreachAutomation.gs into the Apps Script editor.
Modify the script to include your Google Sheet URL and Email Template URLs.
Email Template Setup:

Create a Google Doc for your email template.
Include placeholders such as [FIRST_NAME], [COMPANY_NAME], [ROLE], and [CUHACKING_CORRESPONDENT] where personalization is needed.
Update the TEMPLATE_URLS constant in the script with your Google Doc URL.
Authorize the script:

Run the script in Google Apps Script. The first time you run the script, it will ask for permissions to access Google Sheets and Gmail. Click Authorize and follow the prompts.
Run the automation:

The script will either draft or send emails based on the function call: doEmailAction(EMAIL_ACTION.SEND) for sending or doEmailAction(EMAIL_ACTION.DRAFT) for drafting emails.
Modify the email template key if needed (e.g., 'DEMO', 'COLD', etc.).
How It Works
The script pulls sponsor data from the specified Google Sheet.
It dynamically identifies column letters based on the headers.
Using the template defined in Google Docs, it personalizes each email with sponsor details like the representative’s first name, company name, and role.
Depending on the action (SEND or DRAFT), the emails are either sent or drafted for review.
Example Use Case
Imagine you have a list of 100 sponsors in your Google Sheet. Instead of manually drafting 100 emails, this script will automate the process by:

Personalizing each email based on the data in the sheet.
Drafting or sending the emails using your pre-configured template.
Folder Structure
bash
Copy code
├── README.md
├── cuHackingSponsorshipOutreachAutomation.gs  # Main Google Apps Script file
Contribution
Feel free to open issues or contribute to the project via pull requests.

