Amazon Product Scraper
This project is a Python-based web scraper that extracts product information from Amazon, including product titles, prices, ratings, reviews, and availability status. The data is then saved into a CSV file for further analysis.

Table of Contents
Installation
Usage
Features
Requirements
Contributing
License
Contact
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/amazon-product-scraper.git
cd amazon-product-scraper
Create a virtual environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Make sure you have a compatible version of Python installed (Python 3.6 or above is recommended).

Usage
Edit the HEADERS variable in the script:

You need to provide your User-Agent in the HEADERS dictionary in the script. This is necessary to avoid being blocked by Amazon while scraping.

python
Copy code
HEADERS = ({'User-Agent':'your-user-agent', 'Accept-Language': 'en-US, en;q=0.5'})
Run the script:

Execute the script to start scraping data from Amazon:

bash
Copy code
python amazon_scraper.py
The script will save the extracted data to a CSV file named amazon_data.csv in the project directory.

Features
Product Title Extraction: Extracts the title of each product.
Price Extraction: Captures both regular and deal prices.
Rating and Review Count: Retrieves the product rating and the number of reviews.
Availability Status: Checks whether the product is available for purchase.
Requirements
Python 3.6 or above
requests
beautifulsoup4
lxml
pandas
numpy
You can install the required packages using:

bash
Copy code
pip install -r requirements.txt
Contributing
Contributions are welcome! Please open an issue to discuss what you would like to change. You can also fork this repository and create a pull request with your changes.

