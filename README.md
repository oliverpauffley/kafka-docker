# Docker Kafka
A basic docker-compose file to run a single kafka broker and zookeeper in docker.

## Running
```bash
docker-compose up -d
```

### Enviroment Variables
To create kafka topics when the container is built add the following line to the kafka environment in docker compose.
```yaml
environment:
      KAFKA_CREATE_TOPICS: "Topic1:1:3,Topic2:1:1:compact"
```

### Images
Uses the fantastic images from [wurstmeister](https://github.com/wurstmeister/kafka-docker).

