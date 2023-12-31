# Drug-Orders-Automation

This repository presents a script designed to scan one pharmaceutical e-shop for available drugs. Leveraging web automation tools, the script detects in-stock medications and, upon identifying them, initiates an automated ordering process. 
As some drugs on pharmaceutical e-shops are partly ordered manually by pharmacy employees, this script can help to order essential drugs that are missing in Czechia due to long-term interruptions so that the pharmacy can order sufficient supplies for the upcoming period.

## Features

- Search and scrape drug availability from a pharmaceutical e-shop.
- Convert scraped data from CSV to JSON format for better data manipulation.
- Easily configure drugs to be ordered and their quantities using JSON.
- Automate the process of ordering drugs if they are in stock.

## Python Scripts

### `main.py`

The `main.py` script serves as the entry point of this application. It orchestrates the entire process of searching for and ordering drugs from a pharmaceutical e-shop. You can customize the configuration variables in this script to tailor the automation process according to your requirements.

### `order.py`

The `order.py` script contains the implementation of the `SeleniumOrder` class, which handles the interaction with the e-shop and the automation of ordering drugs. It utilizes web scraping techniques with Selenium to detect drug availability and initiate the ordering process for in-stock medications.

### `json_jobs.py`

The `json_jobs.py` script provides functions to manipulate JSON data. It includes functionalities to convert CSV data to JSON format, open and process JSON files, and perform other tasks related to JSON data manipulation. This script is essential for managing the drug order data in a structured format.

## Files

### `objednat.json`

This JSON file contains a list of drugs that are to be ordered from the e-shop. It specifies the drugs to be ordered and the desired quantities. This file is created during script running.

### `script.log`

The `script.log` file is a log generated by the script during its execution. It provides a detailed record of the script's activity, including information about the scanning process, drug availability checks, and any errors encountered. Reviewing this log can help you monitor the script's behavior and troubleshoot issues.

## License

This project is licensed under the [MIT License](LICENSE).

---

Created by Marketa Dalecka
