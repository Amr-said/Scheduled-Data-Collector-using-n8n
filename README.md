# Scheduled Data Collector using n8n
This project is an automated workflow built with **n8n** to fetch, validate, and store data on a regular schedule into separate Google Sheets.

## Workflow Overview

1. **Schedule Trigger**  
   - Automatically runs at set intervals.

2. **Clear Data**  
   - Clears the previous data from the target sheet to avoid duplication.

3. **Data Fetching**  
   - Sends an HTTP GET request to a public API (likely transportation data) to retrieve fresh records.

4. **Filtering**  
   - Evaluates each record against custom validation rules (e.g., required fields, value ranges).

5. **Data Classification & Storage**  
   - Valid data → appended to a `Filtered Data` Google Sheet  
   - Invalid data → stored in a separate `Invalid Data` Google Sheet

## Technologies Used
- **n8n**
- **Google Sheets**

<img width="1557" height="563" alt="image" src="https://github.com/user-attachments/assets/736acf11-1c3e-45a8-9950-6feed7aacc54" />
