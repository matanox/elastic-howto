# elastic-howto

###checking and manipulating the elastic server on the local (Ubuntu) machine
```
sudo service elasticsearch status
sudo service elasticsearch start
sudo service elasticsearch stop
```

[more details here](https://www.elastic.co/guide/en/elasticsearch/reference/current/setup-service.html#_using_chkconfig)

###browsing your elastic cluster and data with the HQ plugin
http://localhost:9200/_plugin/hq/
don't forget connecting to your elastic cluster of choice by e.g. entering http://localhost:9200 then pressing the connect button
_Note that you can also purge data from the administration portion of the HQ plugin_

###browsing your elastic data and creating dashboards with Kibana:
http://localhost:5601/app/kibana
