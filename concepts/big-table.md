# Big Table
(Hbase and cassandra are modelled on same)
- PB scale thousands of machine
- Goals
    - wide applicability
    - high avaiability
    - high performanace
    - scalability
- Facts: 60+ products of google use big table eg. google search etc


## Data Model:
Sparse, distributed, persistent, multi-dimensional, sorted map

Map index: rowkey, colkey and timestamp

Webtable:

rowkey: "com.cnn.www"
"come.cnn.www": {//rowkey
    "content": {//colkey
        '12321384345': "<html>...<html>",
        '12332499880': "<htmk>...<html>"
    }
    "anchor":{//column family
        "cnnsi.com": "cnn",
        "my.look.ca": "cnn.com"
    }
}