# API reader
## Simple API reader for reading nested values from JSON

Just a simple JSON reader for getting and reading REST API data. This Script was intended to use on my Stock Signals API


```
data = requests.get("<<JSON URL GOES HERE>>")
web_data = data.content
jsonify = json.loads(web_data)
```

for finding all JSON data and keys
```
all_data = FindMarket.find_all_market_data(json_data=<<JSON DATA GOES HERE>>)
all_data_key = FindMarket.find_data_by_key(jsonify, '<<KEY GOES HERE>>')
```