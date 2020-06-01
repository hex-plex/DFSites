# DFSites
This is tool help full in webscrapping
## How to Use
```python
from DFSites import DFSites
url = "https://www.a2oj.com/"  ## This is the url needed to search.
substring = "codeforces"       ## If this is found in the href then it return the hyperreference
maxdepth = 5                   ## (optional) max depth of checking pages by default its 10
init = "Ladders.html"          ## (optional) This specifies which part of the original website is to be searched
obj = DFSites(url,substring,maxdepth,init) ## initializes the site and fetches data
obj.archive                    ## The required data is stored in format of the [hyperreference,Previous page content]
```
## Requirments

> requests, bs4