# cuHacking Sponsorship Outreach Automation

This project automates sponsorship outreach by integrating **Google Sheets** and **Gmail** using **Google Apps Script**. It helps streamline email communication for sponsorships, including drafting and sending personalized emails based on spreadsheet data.

## Features

- **Automated Email Sending/Drafting:** Automatically sends or drafts personalized emails for each sponsor listed in a Google Sheet.
- **Dynamic Email Templates:** Fetches and customizes email templates from Google Docs, replacing placeholders (e.g., `[FIRST_NAME]`, `[COMPANY_NAME]`, etc.) with real values from the spreadsheet.
- **Column Header Mapping:** Dynamically identifies relevant data (e.g., company name, representative's name, email address) by detecting headers in the Google Sheet.
- **Seamless Integration:** Connects Google Sheets and Gmail for efficient outreach, minimizing manual work.

## Setup Instructions

### Prerequisites

- A **Google Account** with access to Google Sheets and Google Docs.
- A Google Sheet with sponsor data. The sheet should include headers such as:
  - **Company Name**
  - **Rep. Full Name**
  - **Role**
  - **Email Address**
  - **cuHacking Correspondent**
- Google Apps Script access.

### Steps

1. **Clone this repository**:
   ```bash
   git clone https://github.com/akshavib/cuHackingSponsorshipOutreachAutomation.git
