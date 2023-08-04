# Amazon Web Scraper


## Introduction
This Python script fetches data from Amazon's website related to PS5 products and saves it in an Excel file. It utilizes the `requests`, `beautifulsoup4`, and `openpyxl` libraries for web scraping and working with Excel files.

## Prerequisites
Make sure you have the following installed:
- Python (version 3.6 or above)
- `requests` library (`pip install requests`)
- `beautifulsoup4` library (`pip install beautifulsoup4`)
- `openpyxl` library (`pip install openpyxl`)

## Execution
1. Set the desired URL in the `url` variable.
2. Run the script.

## Code Explanation
1. The script starts by importing the necessary libraries and defining variables for the URL, headers, and file names.
2. A GET request is sent to the specified URL with custom headers to retrieve the webpage content.
3. If the request is successful (status code 200), the webpage content is saved to an HTML file.
4. The HTML file is then read and parsed using BeautifulSoup.
5. The script finds all div elements with the specified class that contain product information.
6. An Excel workbook is created, and the active sheet is selected.
7. Headers for the product name and price are written to the Excel sheet.
8. The script iterates over the div elements, extracts the product name and price, and writes them to the Excel sheet.
9. The resulting Excel file is saved with a timestamp in the file name.

## Conclusion
By running this script, you will be able to scrape PS5 product or Every page data from Amazon's website and save it in an Excel file for further analysis or processing.
