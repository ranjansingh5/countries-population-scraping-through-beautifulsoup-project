# 🌍 Countries Population Scraper – Worldometer
## 📌 Project Overview

This Python project scrapes the list of countries, their population, and region from the Worldometer website and stores the data in a structured CSV file.

The script uses Requests and BeautifulSoup to collect data and Pandas to organize and save it.

---

## 🔗 Table of Contents

- [Data Source](data-source)
- [Feature](feature)
- [Technologies Used](technologies-used)
- [Project Structure](project-structure)
- [How the Script Works](how-the-script-works)
- [Author](author)

---

## 🌐 Data Source

Website used in this project: https://www.worldometers.info/geography/countries-of-the-world/

---

## 🚀 Features

- Scrapes country rank, name, population, and region
- Processes the data into a Python dictionary
- Stores all records in a Pandas DataFrame
- Exports the results to a CSV file

---

## 🛠️ Technologies Used

- `Python`
- `requests` – for sending HTTP requests
- `BeautifulSoup (bs4)` – for parsing HTML
- `pandas` – for handling and saving data

---

## 📂 Project Structure

countries_population_scraper

├── geography_scraper.ipynb

├── countries_population_2026.csv

└── README.md

---

## ⚙️ How the Script Works

1. Import required libraries: `requests`, `pandas`, `BeautifulSoup`.
2. Create an empty list `countries_info` to store data.
3. Send an HTTP request to the Worldometer countries page.
4. Parse the HTML content using BeautifulSoup.
5. Find the main table containing country data.
6. Loop through each row of the table:
    * Extract rank, country name, population, and region.
    * Store each row as a dictionary.
    * Append to the list `countries_info`.
7. Convert the list of dictionaries into a Pandas DataFrame.
8. Save the DataFrame to a CSV file: `countries_population_2026.csv.`

---

## 📊 Output

countries_population_2026.csv will have the following structure:

|#	 | Country	    | Population	| Region        |
| -- |  ----------- | --------------| ------------- |
|1	 | China	    | 1,425,671,352	| Asia          |
|2	 | India	    | 1,428,627,663	| Asia          | 
|3	 | United States| 339,996,563	| North America |


## 🧑‍💻 Author

Author: Ranjan Singh

Project Type: Web Scraping / Data Collection

Language: Python