# Scrapy
## First Demo Run
Use the follow command line
```
scrapy runspider Demoz.py -o quotes.json
```
## Seconde Demo Run
Use the follow command build project
```
scrapy startproject scrapydemoz
```
Add quotes_spider.py file
Use the follow command line
```
scrapy crawl quotes
```
## scrapy shell
```
scrapy shell "http://quotes.toscrape.com/page/1/"
```
shell command, remenber input the word serialsly or it will conduct error
**Example** if u input **('title')** with the order "**( ) ' ' title**" shell
will overlap "**)**" when u input "**'**" then u must reinput "**)**" after that u input 
**Enter** the shell tell **SyntaxError**
this may be a bug of scrapy shell
```
 response.css('title')
```
## command line argument 

```python
 tag = getattr(self, 'tag', None)
        if tag is not None:
            url = url + 'tag/' + tag
```
command line
```
scrapy crawl quotes -a tag=humor
```

## genspider
using follow command
```
$ scrapy genspider -t crawl scrapyorg scrapy.org
```