# ELK + GRAYLOG

ELK搭配GrayLog使用

此LAB應用以下幾種工具達到紀錄LOG的目的
- FileBeat (收取Log檔案)
- LogStash (Parse Log 檔案
- ElasticSearch_7.10.2 (Log搜尋引擎 + 儲存體)
- GrayLog_5.1.3 (讀取ElasticSearch 讀取Log畫面、搭配Mongodb設定)

# 架構圖如下
![image001](https://github.com/willson2021/ELK_GRAYLOG/assets/79440628/ac36d2cf-40ac-4281-be9f-cf0466b33b19)


# Filebeat 
下載網址 : https://www.elastic.co/downloads/beats/filebeat

# Logstash
下載網址 : https://www.elastic.co/downloads/logstash

# elasticSearch
下載網址 : https://www.elastic.co/downloads/elasticsearch

# GrayLog
因Windows無法安裝故使用Docker來安裝GrayLog
Docker Cmd : docker run --name graylog -d -p 9000:9000 -p 12201:12201/udp -p 1514:1514 graylog/graylog:5.1.3

# Mongodb
下載網址 : https://www.mongodb.com/try/download/community
