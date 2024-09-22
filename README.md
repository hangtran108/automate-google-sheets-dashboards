# Google Sheets Dashboard Automation

This project provides a step-by-step guide for building Google Sheets dashboards that automatically update at your desired time and frequency using Apps Script. If you're looking to streamline your reporting and dashboard processes, it will help you automate tasks like data import, visualization updates and notification systems.

---

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Setup Guide](#setup-guide)

---

## Introduction

This repository is designed to help users automate their Google Sheets dashboards by providing pre-built scripts, functions, and templates. By leveraging Google Apps Script and a few other tools, you can reduce manual work, minimize errors, and create real-time dashboards with dynamic content.

If you’re managing repetitive tasks such as regular data updates, generating charts, or creating dashboards for performance tracking, this project will provide you with the framework to automate it all.

---

## Features

- **Automated Data Imports:** Schedule imported data from a specific Google Bigquery into Google Sheets.
- **Scheduled Refreshes:** Use triggers to periodically update your dashboards.
- **Dynamic Charts and Visualizations:** Automatically update charts based on the latest data.
---

## Prerequisites

Before getting started, ensure you have the following:

- A Google Account with access to Google Sheets and Google Bigquery.
- Basic knowledge of Google Sheets, Google Apps Script, Google Bigquery.
- Familiarity with JavaScript or similar languages (helpful but not mandatory).

---

## Setup Guide

1. **Write queries to extract data you want** on Google Bigquery
2. **Run query**, **download** the dataset and **import CSV file** to a sheet in Google Sheets
3. **Paste query** to a specific cell in a new sheet in your existing Google Sheets file: You can name the sheet whatever you like, in my example, I name it "query" sheet.
5. Click **Extension** -> **Apps Script**
6. Paste the code in the **Code.js**
7. **Change important information** below:
- Name of the sheet containing your query
- The cell containing your query
- The final column number to clear data before displaying the result if you do not want to clear the whole sheet
- Name of the sheet that you want your data to be imported after running your query
8. Choose "**BigQuery API**" service in the **Services** section
9. Click "**Run**" to check if it can run successfully
10. If the code runs successfully, click "**Trigger**" to set up trigger events
11. **Select your options**:
  - For "selecting event source", choose "Time-driven" option
  - For "Select type of time based trigger", choose the frequency you desire to update your data
  - For "Select time of day", choose the time interval to let your query run
  - Click "Save" to create the trigger
 

**DONEEEEE!!!**


