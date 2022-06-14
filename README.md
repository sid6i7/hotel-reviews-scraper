# Hotel Reviews Scraper

Hotel Reviews Scraper is a simple to use web scraper that can scrape hotel reviews from TripAdvisor.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

## Required Libraries:
```bash
pip install selenium, beautifulsoup4, webdriver-manager, pandas
```

## Usage

First run the code to setup the Selenium's chrome driver.
```python
service = Service(ChromeDriverManager().install())
driver = webdriver.Chrome(service=service)
url = 'https://www.tripadvisor.in'
driver.get(url) 
```

Then run the function start_scraping().
```python
start_scraping()
```
![image](https://user-images.githubusercontent.com/92942861/165897388-320d3e91-2d36-445c-bfa6-ee77a502c8aa.png)

Now it will ask for how many hotels to show in the options list
![image](https://user-images.githubusercontent.com/92942861/165897716-3a2a3d66-c1f4-4aca-8186-73c0aadadef6.png)

Finally, it will ask for the hotel name to search for
![image](https://user-images.githubusercontent.com/92942861/165897890-a727053e-8791-44d4-9f36-406b0715a44e.png)

For demonstration, let us search for "Marriott"

This is how the output is going to look like:
![image](https://user-images.githubusercontent.com/92942861/165898831-478dec79-eb53-480c-8d0b-0de0a9bfa01b.png)

After selecting any of the options, the scraper will start to scrape reviews of that hotel and save it as a csv file (in the same directory as the scraper.ipynb file) with the name that u searched for intially.

In our case the name would be: "Marriott.csv"
