# Repository-Figshare
How to automatize extraction of data, metadata from Figshare, the repository used by ACS for supplementary data

## Search data

Examples of searches for "[total synthesis](https://figshare.com/search?q=%3Atitle%3A%20total%20synthesis%20AND%20%3Asearch_term%3Asi_002.zip&sortBy=relevance&sortType=desc&pubPublishDate=last_year&contentTypes=collection,item&itemTypes=3
)" and "[synthesis](https://figshare.com/search?q=%3Atitle%3Asynthesis%20AND%20%3Asearch_term%3Asi_002.zip&sortBy=relevance&sortType=desc&pubPublishDate=last_year&contentTypes=collection,item&itemTypes=3)"

## Download data

example :

```
wget ...
curl -X GET "https://api.figshare.com/v2/articles/3000002" | json_pp -json_opt pretty,canonical>data/test.json
curl -X GET "https://api.figshare.com/v2/articles/3000002" | json_pp -json_opt pretty,canonical>data/test.json
wget "https://api.figshare.com/v2/articles/3000002" | json_pp -json_opt pretty,canonical>data/test.json

```

Surprisingly, the first produces more hits that the later.

## More info

Direct [link](https://chemedata.github.io/Repository-Figshare/): https://chemedata.github.io/Repository-Figshare/


https://github.com/mello99/figshare_API_client_python
