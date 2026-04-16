# 🚀 Web Scraping CLI Tool using Python (BeautifulSoup + Requests)

## 📌 Overview

This project is a **command-line web scraping tool** built using Python that extracts structured data from websites using **BeautifulSoup** and **Requests**.

It allows users to scrape any website URL and store extracted data such as:

* Page title
* Anchor links
* Images
* Headings (H1, H2, H3)
* Paragraph content

The scraped data is stored in a **JSON database**, making it reusable and easy to analyze.

---

## ⚙️ Features

* 🔍 Scrape any website dynamically via CLI input
* 📄 Extract structured HTML data (links, text, images)
* 💾 Store scraped data in JSON format
* 📊 View previously scraped websites in a tabular format
* 🕒 Timestamp tracking for each scraping operation
* 🔁 Prevent duplicate entries with alias handling

---

## 🛠️ Tech Stack

* **Python 3**
* **BeautifulSoup (bs4)**
* **Requests**
* **Selenium (optional for dynamic content)**
* **JSON (data storage)**
* **Beautifultable (CLI visualization)**

---

## 📂 Project Structure

```
├── web_scraping_command_line_tool.py   # Main CLI tool
├── scraped_data.json                  # Stored scraped data
├── requirements.txt                   # Dependencies
├── Web Scraping with BeautifulSoup.py # Basic scraping script
├── README.md
```

---

## 📥 Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/web-scraping-cli-tool.git
cd web-scraping-cli-tool
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the CLI tool:

```bash
python web_scraping_command_line_tool.py
```

### Menu Options:

```
1 → View existing scraped data  
2 → Scrape a new website  
3 → Exit  
```

---

## 🔍 Example

Input:

```
Enter URL: https://en.wikipedia.org/wiki/World_War_II
```

Output:

* Page Title
* List of links
* Headings
* Paragraph content
* Images

Sample stored JSON structure:

```json
{
  "title": "World War II - Wikipedia",
  "all_anchor_href": [...],
  "all_h1_data": [...],
  "all_p_data": [...]
}
```

---

## 🧠 How It Works

* Sends HTTP request using `requests`
* Parses HTML using `BeautifulSoup`
* Extracts tags (`a`, `img`, `h1`, `p`, etc.)
* Stores structured data into JSON
* Displays results via CLI

---

## ⚠️ Limitations

* Does not handle heavy JavaScript-based websites (without Selenium)
* No rate limiting (can be added)
* Basic error handling

---

## 🚀 Future Improvements

* Add async scraping for speed
* Add proxy & rate limiting
* Export data to CSV / database
* Build a web dashboard
* Add scraping scheduler

---

## 📸 Demo

(Add screenshots here — VERY IMPORTANT for recruiters)

---

## 👨‍💻 Author

**Vitthal Misal**

* GitHub: https://github.com/vitthal-misal
* LinkedIn: https://linkedin.com/in/vitthal-misal

---

## ⭐ Why This Project Matters

This project demonstrates:

* Real-world web scraping skills
* Data extraction & automation
* CLI tool development
* File handling & JSON storage

---

## 📜 License

This project is licensed under the MIT License.
