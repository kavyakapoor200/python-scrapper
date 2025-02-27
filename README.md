# python-scrapper
# Python Scraper

## Overview
The **Python Scraper** is a web scraping tool designed to extract product details from Amazon search result pages and product pages. The scraper collects essential product information such as title, price, rating, and seller name, efficiently navigating through multiple search result pages and saving the extracted data in a structured format.

## Features
- Extracts product details like title, price, rating, and seller name.
- Scrapes multiple pages of Amazon search results.
- Implements HTTP request retries for reliability.
- Saves data incrementally and in a final CSV file.
- Prevents scraping blocks with request delays.

## Files in Repository
- **README.md** - Project documentation.
- **amazon_products.csv** - Output file containing extracted product data.
- **web_scraping.ipynb** - Jupyter Notebook used for running the scraper.

## Requirements
Ensure you have the following dependencies installed before running the scraper:

```bash
pip install requests beautifulsoup4 pandas
```

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/kavyakapoor200/python-scrapper.git
   cd python-scrapper
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the script to start scraping Amazon product details:
   ```bash
   python scraper.py
   ```
2. The extracted product details will be saved incrementally as `amazon_products_partial.csv` and the final dataset as `amazon_products.csv`.

## Example Output
Sample CSV format:
```
Product Name,Price,Rating,Seller Name
"Example Product","$49.99","4.5","Example Seller"
```

## Notes
- The scraper uses request retries and delays to prevent blocking.
- Scraping Amazon may violate their Terms of Service; use it responsibly.
- Consider using **Amazon’s API** for a legal and efficient alternative.

## License
This project is licensed under the MIT License.

## Disclaimer
This scraper is intended for educational purposes only. Scraping Amazon may violate their Terms of Service. Use at your own risk.

## Author
[kavyakapoor200](https://github.com/kavyakapoor200)

