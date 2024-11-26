# Steam Reviews Scrapper

A program to scrape game reviews from Steam game platform.

## Pre-start

Before starting, please make sure all properties inside app.properties file are correct.

The app.properties file contains several properties, such as:

- **scrapper.url:** The url of steam game reviews you want to scrape
- **scrapper.rows_to_scroll:** The number of rows you want to scroll, this number will affect numbers of scrapped data
- **csv.path:** The path to csv file, which is the file to save the scrapping result

For reference, the default values of app.properties are:

```properties
[ScrapperSection]
scrapper.url=https://steamcommunity.com/app/1172470/reviews/?browsefilter=toprated&snr=1_5_100010_
scrapper.rows_to_scroll=1100

[CSVSection]
csv.path=apex_reviews.csv
```

## Setup

The scrapping program uses Jupyter Notebook with Python version 3.11.7. To run this program, you use either global python environment or python virtual environment.

If you prefer to use python virtual environment you can do the following instructions:<br>

1. Create new Python virtual environtment

```bash
python -m venv <path_to_env>
```

2. Activate the virtual environment

Windows:

```bash
<path_to_env>/Scripts/activate
```

Mac & Linux:

```bash
source <path_to_env>/bin/activate
```

3. Install required python modules

```bash
pip install -r requirements.txt
```

4. Run the jupyter notebook

```bash
jupyter execute scraper.ipynb
```

## Others

This project also consist of two different machine learning algorithms you can try on! There are **Naive Bayes Classifier** and **Support Vector Classifier** algorithms. From these two machine learning algorithms, you can compare and see what the differences!
