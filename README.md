# Singlish to Sinhala Translator - Automation Testing

## Project Overview
This project is part of the **IT3040 - Information Technology Project Management (ITPM)** module. The objective is to perform quality assurance testing on a live Singlish-to-Sinhala transliteration tool. The project identifies 50 specific failure scenarios (negative test cases) across 24 different Singlish input categories and automates the validation process using Playwright.

## Student Information
* **Name:**PERERA S.H.K.S
* **Registration Number:** IT23653672
* **Module:** IT3040 - ITPM

## Features
- **Negative Testing:** Focused on identifying weaknesses in the transliteration logic.
- **Automation:** Uses Python and Playwright to automate the interaction with the web-based translator.
- **Reporting:** Generates an Excel report containing Singlish inputs, expected Sinhala outputs, actual outputs from the system, and the pass/fail status.

## Technologies Used
- **Language:** Python 3.x
- **Automation Framework:** Playwright
- **Data Handling:** Pandas, Openpyxl (for Excel integration)

## Installation & Setup

1. **Clone or Extract the Project:**
   Ensure all project files are in a dedicated folder.

2. **Install Dependencies:**
   Run the following commands in your terminal:
   ```bash
   pip install pandas openpyxl playwright
   playwright install
   ```

## How to Run the Test Automation

To execute the automation script and update the Excel report, run the following command in the terminal:

```bash
python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --save-every 1 --keep-open
```

### Command Arguments:
- `--excel`: Path to the input Excel file containing test cases.
- `--url`: The URL of the translator application.
- `--wait-ms`: Time to wait for the translator to process the input.
- `--save-every`: Frequency of saving the Excel file during processing.
- `--keep-open`: Keeps the browser window open after execution for inspection.

## Folder Structure
- `test_automation.py`: The core automation script.
- `Assignment 1 - Test cases.xlsx`: Finalized test case document with 50 failure scenarios.
- `README.md`: Project documentation and execution guide.

## Conclusion
The results documented in the Excel file demonstrate that while the translator handles standard Singlish well, it struggles with highly informal chat-style spellings, clipped forms, and specific numeric suffixes.
