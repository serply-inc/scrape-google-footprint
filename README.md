# Scraping Google Footprint Using Python
Simple script to scrape Google Advanced Search Operators for finding backlink and posting opportunities based on [Useful Google Advanced Search Operators For SEO Guide](https://blog.goog.io/seo/2020/10/30/useful-google-advance-search-operators-for-seo.html)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Python3+

```
https://www.python.org/downloads/
```

### Installing

```bash
# clone repo
git pull https://github.com/googio/scrape-google-footprint.git
# install requirements
pip install -r requirements.txt
# modify query in search.py and run script
python scrape.py
```

## Features

* [Python3](https://www.python.org/) - Python is a programming language that lets you work quickly
and integrate systems more effectively.
* [Pip](https://pip.pypa.io/en/stable/) - The Python Package Installer
* [Requests](https://requests.readthedocs.io/en/master/) - HTTP for Humans
* [Beautiful Soup](https://requests.readthedocs.io/en/master/) - a Python library for pulling data out of HTML and XML files
* [Google Search API](https://googio.io/) - an API for scraping unlimited Google search results

## Footprints

The footprint used are in the [footprints folder](footprints)

- [x] [articles](footprints/article.txt)
- [x] [blogs](footprints/blog.txt)
- [x] [bookmarks](footprints/bookmark.txt)
- [x] [directory](footprints/directory.txt)
- [x] [drupal](footprints/drupal.txt)
- [x] [edu](footprints/edu.txt)
- [x] [forums](footprints/forums.txt)
- [x] [guestbooks](footprints/guestbook.txt)
- [x] [image](footprints/image.txt)
- [x] [indexer](footprints/indexer.txt)
- [x] [microblogs](footprints/microblog.txt)
- [x] [pingback](footprints/pingback.txt)
- [x] [social networks](footprints/socialnetwork.txt)
- [x] [trackbacks](footprints/trackback.txt)
- [x] [videosite](footprints/videosite.txt)
- [x] [wiki](footprints/wiki.txt)

## Usage
The script requires two argument, `footprint` and `keyword`. Footprint is the name of the footprints you want to use, defaults to `edu.txt`. The keyword is the keywords you want to search for.

### Example 1: searching for the keywords "best crossfit workout" with the footpints of edu.txt
[example console output](#console_output)
```bash
python3 scrape.py --footprint edu.txt --keywords "best crossfit workout"
```

### Example 2: searching for the keywords "iPhone review" with the footpints of guestbook.txt 
```bash
python3 scrape.py --footprint guestbook.txt --keywords "iPhone reviews"
```

## Results

The results are saved into [results.txt](results.txt)

### console output
```bash
Scraping footprint: "Powered by Movable Type" "You may use HTML tags for style" , keyword: "best crossfit workout"
Found 9 results.
Scraping footprint: "powered by Mephisto" "a response" -"are closed for" Email Address Website , keyword: "best crossfit workout"
Found 67 results.
Scraping footprint: "Lisa kommentaar" "Kommentaare veel pole." , keyword: "best crossfit workout"
Found 31 results.
Scraping footprint: "Zostaw komentarz" , keyword: "best crossfit workout"
Found 75 results.
Scraping footprint: "Your email address will not be published. Required fields are marked" , keyword: "best crossfit workout"
Found 149 results.
Scraping footprint: "powered by Serendipity" "Remember Information?" , keyword: "best crossfit workout"
Scraping footprint: "Email addresses are never displayed, but they are required to confirm your comments" , keyword: "best crossfit workout"
Found 100 results.
Scraping footprint: "Add a comment" Website , keyword: "best crossfit workout"
Found 137 results.
Scraping footprint: site:.blogspot.es , keyword: "best crossfit workout"
Found 124 results.
Scraping footprint: "add new comment" "what is the first word in the phrase" , keyword: "best crossfit workout"
Found 19 results.
Scraping footprint: "Powered by s9y" "add comment" , keyword: "best crossfit workout"
Found 4 results.
```

## CAPTCHA

<img src="img/reCAPTCHA-logo@2x.png" width="100">

Eventually you will run into CATPCHAs. Consider using a proxy or a service like [Googio](https://goog.io/)



## Contributing

## Versioning

## Authors

* **googio** - *Initial work* - [Googio](https://goog.io/)

## License
[Apache license 2.0](LICENSE)

## Acknowledgments
