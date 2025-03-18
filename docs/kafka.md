`sh zookeeper-server-start.sh ../config/zookeeper.properties` # Start Zookeeper
`sh kafka-server-start.sh ../config/server.properties` # Start Kafka
`sh kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic notifications` # Create a topic
`sh kafka-console-producer.sh --broker-list localhost:9092 --topic notifications` # Start a producer
`sh kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic notifications --from-beginning` # Start a consumer
```
export BOOTSTRAP_SERVERS="6.tcp.eu.ngrok.io:17396"
export SECURITY_PROTOCOL="PLAINTEXT"
export SESSION_TIMEOUT_MS="45000"
export TOPIC_NAME="notifications"
export PREFERRED_BROKER="local-broker"
```

Spring boot
```
DB_HOST=mysql-b48cc93e-fa33-4420-a155-bc653b4d46be-wso2con24246880145-c.l.aivencloud.com
DB_NAME=defaultdb
DB_PASSWORD=AVNS_K9ABgz-gyamXRs1oSDH
DB_PORT=24901
DB_USERNAME=avnadmin
```

```sh
export DB_HOST=mysql-b48cc93e-fa33-4420-a155-bc653b4d46be-wso2con24246880145-c.l.aivencloud.com
export DB_NAME=defaultdb
export DB_PASSWORD=AVNS_K9ABgz-gyamXRs1oSDH
export DB_PORT=24901
export DB_USERNAME=avnadmin
```