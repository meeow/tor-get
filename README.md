# tor-get
Simple API for scraping raw HTML using TOR

## Dependencies: 
- Tor must be running in the background.
- pysocks package
- stem package
- python 2.7

## API:
 @param urls: list of urls to scrape
 
 @param searchnum:
 
   'all': all keywords must be present in the html file corresponding to url
   
   \d: at least searchnum number of keywords must be present 
   
 @param keywords: list of keywords to search for
 
 @return: list where each element is one html page
 
get_html(urls, searchnum='all' , keywords=None)
