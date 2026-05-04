# Playwright_Assignment1_Option1
The main objective of this assignment is to assess how accurately the application available at the following link converts chat-style Singlish input into Sinhala output: https://www.pixelssuite.com/chat-translator

# DESCRIPTION
This project focuses on automated testing of the PixelSuite Singlish to Sinhala translation system.  
The objective of the assignment is to evaluate how accurately the system converts chat-style Singlish input into Sinhala output.

A total of 50 negative test cases were designed to identify weaknesses in the system.  
All test cases were automated using Playwright and the results were recorded in the provided Excel file.

# REQUIREMENTS

Python 3.12.0
pip (latest version)
Playwright
openpyxl

# INSTALLATION

python -m pip install -U pip
python -m pip install playwright openpyxl
python -m playwright install

# RUN AUTOMATION
python test_automation.py --excel "Assignment 1 - Test cases-IT23861336.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1

# TEST_AUTOMATION.PY CHANGES
The original automation script was modified with minimal changes to improve stability and ensure complete execution of all test cases:
The page is reloaded for each test case to prevent UI inconsistencies
Action button click is handled safely using try-except
Empty outputs are handled gracefully without terminating execution


