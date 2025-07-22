# Jiomart-Website-Scraper
🛏️ Jiomart Bedding Scraper
This Python script uses Selenium and BeautifulSoup to scrape bedding products from JioMart. It extracts essential product details like title, price, image URL, discount, and product page link.

📌 Features
Headless browser automation using Selenium

Scrolls through the product page to load more items

Parses product cards using BeautifulSoup

Extracts:

Product title

Price

Product link

Image URL

Discount (if available)

Combined product text

🛠️ Dependencies
Install the following Python libraries before running the script:

bash
Copy
Edit
pip install selenium beautifulsoup4
Also, make sure you have Chrome and ChromeDriver installed and accessible via your system's PATH.

🚀 How to Use
Clone or download the script.

Run the function scrape_jiomart_bedding() in your Python environment.

The function returns a list of dictionaries, each containing product details.

Example
python
Copy
Edit
from jiomart_scraper import scrape_jiomart_bedding

products = scrape_jiomart_bedding()
for product in products:
    print(product)
📦 Output Format
Each dictionary in the returned list contains:

python
Copy
Edit
{
    "product_title": "Example Bedding Set",
    "product_price": "₹999",
    "product_link": "https://www.jiomart.com/p/example",
    "product_image_link": "https://example.com/image.jpg",
    "product_rating": "N/A",
    "product_discount": "20% OFF",
    "product_text": "Full description text extracted from the card"
}
📋 Notes
Ratings are currently set to "N/A" as they are not available on the Jiomart site.

If Jiomart changes its site structure, the scraper may need to be updated.

📄 License
This project is for educational and research purposes only.
