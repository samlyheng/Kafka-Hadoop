# Kafka-Hadoop
Hadoop data ingestion with Kafka
# How to run Hadoop data ingestion with Kafka
# 1. Make sure all Hadoop services are up
# 2. Navigate to the Kafka directory
# 3. Start Zookeeper service
Run: zookeeper-server-start config/zookeeper.properties
# 4. Start Kafka service
Run: kafka-server-start config/server.properties
# 5. Create Topic
Run: bin/kafka-topics.sh --bootstrap-server localhost:9092 --topic my_topic --describe
# 6. To Check Topic
Run: bin/kafka-topics.sh --bootstrap-server localhost:9092 --topic my_topic --describe
# 7. To Sent Message
Run: bin/kafka-console-producer.sh --broker-list localhost:9092 --topic my_topic
# 8. To Check message
Run: bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic my_topic --from-beginning
