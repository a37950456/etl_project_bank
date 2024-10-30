# Acquiring and Processing Information on the World's Largest Banks

## Project Overview

In this project, you will apply all the skills acquired throughout the course and your knowledge of basic Python. You will work with real-world data and perform the operations of Extraction, Transformation, and Loading (ETL) as needed.

## Disclaimer

Cloud IDE is not a persistent platform, and you will lose your progress every time you restart this lab. We recommend saving a copy of your file on your local machine to prevent data loss.

## Project Scenario

You have been hired as a data engineer by a research organization. Your task is to create a script that compiles a list of the top 10 largest banks in the world ranked by market capitalization in billion USD. Additionally, you need to transform and store the data in GBP, EUR, and INR, based on exchange rate information available in a CSV file. The processed information should be saved locally in a CSV format and as a database table.

Your job is to create an automated system to generate this information so that it can be executed every financial quarter to prepare the report.

### Project Details

- **Code Name**: `banks_project.py`
- **Data URL**: [Wikipedia - List of Largest Banks](https://web.archive.org/web/20230908091635/https://en.wikipedia.org/wiki/List_of_largest_banks)
- **Exchange Rate CSV Path**: [Exchange Rates CSV](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0221EN-Coursera/labs/v2/exchange_rate.csv)
- **Table Attributes (upon Extraction)**: Name, MC_USD_Billion
- **Table Attributes (Final)**: Name, MC_USD_Billion, MC_GBP_Billion, MC_EUR_Billion, MC_INR_Billion
- **Output CSV Path**: `./Largest_banks_data.csv`
- **Database Name**: `Banks.db`
- **Table Name**: `Largest_banks`
- **Log File**: `code_log.txt`

## Project Tasks

### Task 1: Logging
- Write a function `log_progress()` to log the progress of the code at different stages in a file `code_log.txt`.

### Task 2: Data Extraction
- Extract tabular information from the given URL under the heading 'By market capitalization' and save it to a DataFrame.
  - Inspect the webpage and identify the position and pattern of the tabular information in the HTML code.
  - Write a function `extract()` to perform the required data extraction.
  - Execute a function call to `extract()` and verify the output.

### Task 3: Data Transformation
- Transform the DataFrame by adding columns for Market Capitalization in GBP, EUR, and INR, rounded to 2 decimal places, based on the exchange rate information.
  - Write a function `transform()` to perform the transformation.
  - Execute a function call to `transform()` and verify the output.

### Task 4: Load to CSV
- Load the transformed DataFrame to an output CSV file.
  - Write a function `load_to_csv()`, execute a function call, and verify the output.

### Task 5: Load to Database
- Load the transformed DataFrame to an SQL database server as a table.
  - Write a function `load_to_db()`, execute a function call, and verify the output.

### Task 6: Query the Database
- Run queries on the database table.
  - Write a function `query_db()`, execute a given set of queries, and verify the output.

### Task 7: Verify Logging
- Ensure that log entries have been completed at all stages by checking the contents of the file `code_log.txt`.

## Conclusion

This project will help you develop practical skills in handling ETL processes, managing data transformations, and automating data workflows using Python.