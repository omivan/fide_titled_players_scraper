# FIDE Titled Players Scraper

This is a scraper for titled FIDE players to extract information from the FIDE website about the year they received their respective FIDE titles.

## Prerequisites

Before running the notebook, install the required dependencies:

```pip install -r requirements.txt```


Before running the scraper, follow these steps:

1. **Download the XML File**

   - Go to [FIDE Ratings List](https://ratings.fide.com/download_lists.phtml).
   - Download the most relevant file in **XML format**.
   - Place the downloaded XML file in the **root** of the project.
   - Update the `INPUT_FILE` variable in the script to match the filename.

2. **Set Up ChromeDriver**

   - Ensure you have **Google Chrome** installed.
   - Download the appropriate **ChromeDriver** for your Chrome version from [ChromeDriver](https://sites.google.com/chromium.org/driver/).
   - Install it on your system and note its path.
   - Update the `CHROMEDRIVER_PATH` variable in the script to the correct path.

## Running the Scraper
Open `main.ipynb` in Jupyter Notebook and **Run All Cells**. The scraping process may take some time, as it gathers data for all titled players.

## Output

- The script will generate a **CSV file** as specified in the `OUTPUT_FILE` variable.
- The CSV will contain:
  - One-hot encoded variables indicating whether a player has a specific FIDE title.
  - The year in which the player received each title (if applicable).

