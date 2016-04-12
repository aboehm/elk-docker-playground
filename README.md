# ELK playground

Small shell script for creating a small Elasticsearch Cluster with Kibana with Docker.

## Architecture

3 Elasticsearch Nodes connected as cluster _es-cluster0_
- _es0_ (Master)
- _es1_
- _es2_

```
 kibana (localhost:5601)
    ^
    |
    v
   es0 (localhost:9200)
  /   \
es1   es2
```

## Usage

Checkout git repository and run the script with different options.

```
elk-playground (start|stop|init|kill|rm)

  init  Initialize the containers and download images
  rm    Delete initialized containers
  kill  Kill running containers
  start Startup the initialized containers
  stop  Stop the running containers
```

Access Elasticsearch through http://localhost:9200 and Kibana over http://localhost:5601.
