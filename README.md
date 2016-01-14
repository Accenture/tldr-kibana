# Introduction

This container provides a Kibana frontend. Requires the tldr/logbox container as that's the one that provides the ElasticSearch and Logstash dependencies.

# Building

```
docker build -t tldr/kibana .
```

# Running

```
docker run -d -p 5601:5601 -h kibana --name kibana -e ELASTICSEARCH_URL=http://localhost:9200 tldr/kibana
```