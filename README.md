# Price-Argus

Panoptes Argus was a giant from the greek mythology, who had 100 eyes to monitor the doings of people. This project does somethisthing similar with the prices of products. 
This project provides a user interface to interact with an automated price tracking web scraper. Currently the tracker scrapes amazon.ca, but could be configured to scrape multiple sources.

### auth.json

We need to ill in our [Bright Data Scraping Browser](https://brightdata.com/products/scraping-browser) credentials in a `backend/scraper/auth.json` file (see `auth_example.json`).
Bright data is a web scraping browser, that I have used in this project.

## Setting Up Automation

To automate the collection of prices from this software simply run the `scheduler/main.py` file at your desired increment while the python flask backend is running.

### Windows

I have created a simple `.bat` script called `run.bat` that you can schedule to execute using the Windows Task Scheduler that will automatically run the backend api and send the appropriate request to it.
