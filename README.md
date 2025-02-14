# shopify

Simple scraper to extract all products from shopify sites

## Requirements

Python 3

## Usage

### Saving result as csv

```bash
python3 shopify.py --url [site's url] > products.csv
```

### Saving result as json 

```bash
python3 shopify.py --output-format json --url [site's url] > products.json
```

### Listing collections

```bash
python3 shopify.py --list-collections --url [site's url] > products.csv
```

### Scraping products only in given collections

```bash
python3 shopify.py -c col1,col2,col3 --url [site's url] > products.csv
python3 shopify.py -c men,for-him,hats --url https://www.qalo.com > products.csv
```

### Shopify URLs in batch

```bash
python3 shopify.py --batch [comma separated file path] > products.csv
python3 shopify.py --batch 150urls.txt > products.csv
```