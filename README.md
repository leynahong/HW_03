# Scraping from eBay
**Read more on how my 'ebay-dl.py' file scrapes product data from eBay and returns a JSON file for any product of interest.**

---

## What it does

The 'ebay-dl.py' file will take a search term as an input and return a JSON file with data from the first 10 pages of search results. Because the file is written with argparse, this will work for any search term on eBay. Outlined below are the instructions on how to look up any search term. 

The python file will produce the following data: 'name', 'price', 'status', 'shipping', 'free_returns', and 'items_sold'.

## How it works

The 'ebay-dl.py' file does the following:
1. sets command line arguments
2. loops over the eBay webpages 
    1. builds the url
    2. downloads the html
    3. processes the html
    4. loops over the items in the page
3. writes the JSON file for the search term

To get a JSON file for any search term, run the following command in the terminal:
<pre><code>python3 ebay-dl.py 'search term'
</code></pre>

To get the three JSON files I produced, run the following commands in the terminal:

<pre><code>python3 ebay-dl.py 'phone case'
</code></pre>

This will produce the [phone case.json](https://github.com/leynahong/HW_03/blob/main/phone%20case.json) file.

<pre><code>python3 ebay-dl.py 'masks'
</code></pre>

This will produce the [masks.json](https://github.com/leynahong/HW_03/blob/main/masks.json) file.

<pre><code>python3 ebay-dl.py 'mug'
</code></pre>

This will produce the [mug.json](https://github.com/leynahong/HW_03/blob/main/mug.json) file.

---

**NOTE:** [here](https://github.com/mikeizbicki/cmc-csci040/tree/2021fall/hw_03) is the link to the course project.
 
