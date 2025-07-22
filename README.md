# 🛏️ Jiomart Bedding Scraper

This project is a web scraper built with **Selenium** and **BeautifulSoup** to extract bedding product listings from [JioMart Bedding Section](https://www.jiomart.com/c/homeandkitchen/home-furnishing/bedding/31421). It scrolls the page, waits for elements to load, and extracts details like product title, price, discount, and more.

## 🚀 Features

- ✅ Headless browser scraping using Selenium  
- ✅ Simulates scrolling to load more products  
- ✅ Parses product details with BeautifulSoup  
- ✅ Collects:
  - Product title
  - Price
  - Product URL
  - Image link
  - Discount (if any)
  - Raw product text

## 🧰 Requirements

Install the required packages:

pip install selenium beautifulsoup4

markdown
Copy
Edit

Make sure **Google Chrome** and the corresponding version of **ChromeDriver** are installed and accessible in your system's PATH.

## 📄 Usage

```python
from scraper import scrape_jiomart_bedding

products = scrape_jiomart_bedding()

for product in products:
    print(product)
📝 Output Example
Each product is returned as a dictionary:

python
Copy
Edit
{
    "product_title": "Floral Cotton Double Bedsheet",
    "product_price": "₹799",
    "product_link": "https://www.jiomart.com/p/example-product",
    "product_image_link": "https://example.com/image.jpg",
    "product_rating": "N/A",
    "product_discount": "15% OFF",
    "product_text": "Floral Cotton Double Bedsheet ₹799 15% OFF"
}
⚠️ Disclaimer
This script is for educational and personal research use only.

Frequent scraping may violate JioMart's Terms of Service.

Always respect robots.txt and rate-limit your requests.

📌 To Do
 Add CSV/JSON export

 Implement pagination-based loading

 Add support for other JioMart categories

📃 License
MIT License © 2025
Feel free to fork, modify, and use this script responsibly.

yaml
Copy
Edit

---

Let me know if you want the same in `.md` file format or need additional badges (e.g. Python version, license, etc.) f
