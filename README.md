# searchresult.dev
Scrape Search Result from Any website using our easy to use API using [Search Result API](https://searchresult.dev/)

## Quick start - Python
This example runs a search for "web" using your API key, at Hacker news search.

```python
import requests

# Copy your API key from your dashboard (After logged into https://searchresult.dev/), go to Profile > API Keys > NEW API KEY  & place it instead of '*****' in the below header section.

headers = {
    'Authorization': 'Api-Key *****',
}

# search result url with query string
data={'url': 'https://hn.algolia.com/?q=web'}
result = requests.get('https://www.searchresult.dev/search_api/api/', headers=headers,   params=data )
print(result)
```

### Result:
```
[
	{"url":"https://news.ycombinator.com/item?id=28550764","title":"A search engine that favors text-heavy sites and punishes modern web design","text":"(https://search.marginalia.nu/) 3441 points | Funes- | 1 year ago | 717 comments"},
	{"url":"https://news.ycombinator.com/item?id=8624160","title":"Launching in 2015: A Certificate Authority to Encrypt the Entire Web","text":"(https://www.eff.org/deeplinks/2014/11/certificate-authority-encrypt-entire-web) 2019 points | mariusz79 | 8 years ago | 411 comments"},
	{"url":"https://news.ycombinator.com/item?id=26271117","title":"Show HN: Redbean Single-file distributable web server","text":"(https://justine.lol/redbean/index.html) 1998 points | jart | 2 years ago | 249 comments"},
. . . 

	{"url":"https://news.ycombinator.com/item?id=22180559","title":"Congrats! Web scraping is legal! (US precedent)","text":"(https://parsers.me/us-court-fully-legalized-website-scraping-and-technically-prohibited-it/) 1057 points | ehurynovich | 3 years ago | 388 comments"}
]
```
## Using Curl
curl https://www.searchresult.dev/search_api/api/?url=https://hn.algolia.com/?q=web -H "Authorization: Api-Key place-your-key-here"

## For other language code samples . . 
Convert the above curl commands to Python, JavaScript, PHP, R, Go, C#, Ruby, Rust, Elixir, Java, etc using https://curlconverter.com/ or similar tool.

## Change log
2022-11-27 @ 0.1.0
 - Developed core AI engine 
 - More to come
