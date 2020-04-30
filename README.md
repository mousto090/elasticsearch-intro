# Getting Started with Elasticsearch

A getting started with elasticsearch from [egghead.io](https://egghead.io/courses/get-started-with-elasticsearch)

## Setting Up
Install [docker](https://www.docker.com/), [elasticsearch](https://www.elastic.co/elasticsearch/) and [kibana server](https://www.elastic.co/kibana)

The `docker-compose.yml` allow to set up a basic [elasticsearch](https://www.elastic.co/elasticsearch/) and [kibana server](https://www.elastic.co/kibana)

Make sure docker is runing then run `docker-compose up`

Elasticsearch will be listening at http://localhost:9200
Kibana will be listening at http://localhost:5601

## Data
The Simpsons [dataset](https://www.kaggle.com/wcukierski/the-simpsons-by-the-data) is used for the demo and also availible in `simpsons_dataset` folder

The datasets is loaded in elasticsearch using [logstash](https://www.elastic.co/downloads/logstash) 

Install [logstash](https://www.elastic.co/downloads/logstash) 

The logstash config for each dataset in `simpsons_dataset/logstash` folder

`cd simpsons_dataset/logstash` then run `logstash -f simpsons_dataset/logstash/file_name.conf` for each logstash config file, first, you will need to ajust the `path` in each file 