# python-webcrawling-basiscs
Webcrawling with python according to [https://www.digitalocean.com/community/tutorials/how-to-crawl-a-web-page-with-scrapy-and-python-3](www.digitalocean.com/community/tutorials/how-to-crawl-a-web-page-with-scrapy-and-python-3)

# Step 1 - Creating a Basic Scraper
We are using Scrapy to build the scraper. If it is not already installed run

```
$ pip install scrapy
```
After that we implement a first BrickSetSpider class.

```python
class BrickSetSpider(scrapy.Spider):
    name = "brickset_spider"
    start_urls = ['http://brickset.com/sets/year-2016']
```

We can run it with scrapys own CLI.

```
scrapy runspider scraper.py
```
