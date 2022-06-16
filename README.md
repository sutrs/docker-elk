# docker ELK -  ElasticSearch, Logstash, and Kibana

## Tutorial
[Docker ELK : ElasticSearch, Logstash, and Kibana]

**Docker compose**
There are couple of ways to install the ELK stack with Docker. We can either pull ELK's individual images and run the containers separately or use Docker Compose to build the images and run the containers.

In this post, we'll run docker-compose

First, clone the repo:

$ git clone https://github.com/sutrs/docker-elk.git

Then, run "docker-compose":

$ cd docker-elk

$ docker-compose up

Check ELK containers
$ docker ps
$ lsof -PiTCP -sTCP:LISTEN

By default, the stack exposes the following ports:

5000: Logstash will listen for any TCP input on port 5000

9200: Elasticsearch for HTTP REST API
![image](https://user-images.githubusercontent.com/43083820/174087422-e271f716-febb-4601-919b-afa5795e25e8.png)



9300: Elasticsearch TCP nodes communication

5601: Kibana web UI

