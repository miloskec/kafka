# Kafka Microservice

## Setup Instructions

1. Navigate to the kafka directory:
    ```sh
    cd kafka
    ```
2. Start the Kafka service:
    ```sh
    docker-compose up -d
    ```
3. Create the Kafka topic:
    ```sh
    docker exec -it kafka /bin/bash
    kafka-topics.sh --create --topic user_created_topic --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
    ```

## Environment Configuration

Copy the content from the `.env.example` to the `.env` file and configure the environment variables as needed.

## Additional Commands

To stop the service:
```sh
docker-compose down
```
 
  
   