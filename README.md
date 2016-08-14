# elastic-howto

###checking and manipulating the elastic server on the local (Ubuntu) machine
```
sudo service elasticsearch status
sudo service elasticsearch start
sudo service elasticsearch stop
```

[more details here](https://www.elastic.co/guide/en/elasticsearch/reference/current/setup-service.html#_using_chkconfig).

you may also query status against a running cluster via e.g. http://localhost:9200/_stats/

###browsing your elastic cluster and data with the HQ plugin
http://localhost:9200/_plugin/hq/ (don't forget connecting to your elastic cluster of choice by e.g. entering http://localhost:9200 then pressing the connect button)

_Note that you can also purge data from the [indices portion](http://localhost:9200/_plugin/hq/#indices) of the HQ plugin UI_

###browsing your elastic data and creating dashboards with Kibana:
http://localhost:5601/app/kibana
[some kibana settings for using elastic indices](https://www.elastic.co/guide/en/kibana/current/settings.html)

## creating and indexing data

[mappings play a role](https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping.html)

[hopefully see also here](https://discuss.elastic.co/t/viewing-data-not-collected-through-logstash-but-rather-independently-shipped-into-elastic/53936/2)
