# Web Scraping Table Data Using Python

## Project Overview

This project demonstrates how to scrape tabular data from a website using Python. The scraped data is extracted from an HTML table and saved into a structured CSV file using Pandas. The process involves locating the table using BeautifulSoup, parsing the rows and columns, and exporting the data for external use.

## Features

* Web scraping using `requests` and `BeautifulSoup`
* Dynamic HTML table parsing
* Data cleaning and organization using `pandas`
* Export of data to a `.csv` file

## Technologies Used

* Python 3
* `requests`
* `BeautifulSoup4`
* `pandas`

## Steps Followed

1. **Importing Libraries**
   The project begins by importing the necessary Python libraries:

   * `requests` for fetching the webpage content
   * `BeautifulSoup` from `bs4` for parsing the HTML
   * `pandas` for data manipulation and storage

2. **Specifying the URL**
   The target webpage URL containing the table was specified.

3. **Fetching and Parsing the Page**
   The HTML content of the page was fetched using `requests` and parsed using `BeautifulSoup`.

4. **Locating the Table**
   The relevant table was identified using either a tag (like `<table>`) or a specific class name.

5. **Extracting the Headers**
   The table headers were extracted and stored as column names in a pandas DataFrame.

6. **Extracting Row Data**
   Each row was parsed to get individual cell data. These rows were then appended to the DataFrame.

7. **Exporting to CSV**
   The final DataFrame was exported to a CSV file for later use.

## How to Run

1. Clone the repository or copy the script to your local machine.
2. Install the required libraries:

   ```bash
   pip install requests beautifulsoup4 pandas
   ```
3. Run the Python script:

   ```bash
   python your_script_name.py
   ```
4. The output CSV file will be saved in the same directory.

## Output

The resulting CSV file contains structured data from the HTML table, ready for analysis or reporting.

## Notes

* Make sure the target website allows scraping and that your script complies with its `robots.txt` rules.
* The HTML structure of the target website may change over time, so the selectors might need to be updated accordingly.

