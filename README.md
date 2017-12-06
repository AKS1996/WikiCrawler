# WikiCrawler

Sample Java Web Crawler. Uses JSoup library.
You can specify either number of files to be downloaded or max data downloaded(I had a 2G connection that time).

Also includes proxy authentication.
**NOTE:** Doesn't downloads images/other resources. 

## Algorithm
1. Download a base URL
2. Scrap all 'http://' strings out of it(the links)
3. Recursively download the links until some stopping condition is met(file count or total download size)
4. Also maintains a list of loaded links, to prevent re-downloading
