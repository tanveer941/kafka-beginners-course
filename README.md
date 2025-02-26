# Kafka for Beginners

This is a companion repository for the [Kafka for Beginners course](https://links.datacumulus.com/apache-kafka-coupon) by Conduktor

![Conduktor](images/kafka-beginners.png)

## Content
- Basics of Kafka Java Programming
- Wikimedia Producer
- OpenSearch Consumer
- Kafka Streams Sample Application

# By Conduktor

[Conduktor](https://www.conduktor.io) is about making Kafka accessible to everyone. Check out our free Kafka learning website [Kafkademy](https://kafkademy.com/) and our Apache Kafka Desktop Client [Conduktor DevTools](https://conduktor.io/download)

![Conduktor](https://www.conduktor.io/images/logo.svg)

~/kafka_2.13-3.9.0/bin/kafka-storage.sh random-uuid
~/kafka_2.13-3.9.0/bin/kafka-storage.sh format -t sq6ZYgvlT9u1HaBmt6aGfg -c ~/kafka_2.13-3.9.0/config/kraft/server.properties

~/kafka_2.13-3.9.0/bin/kafka-server-start.sh ~/kafka_2.13-3.9.0/config/kraft/server.properties

kafka-topics.sh --bootstrap-server localhost:9092 --topic demo_java --create
kafka-topics.sh --bootstrap-server localhost:9092 --list
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic demo_java --from-beginning


kafka-topics.sh --bootstrap-server localhost:9092 --topic demo_javap --create --replication-factor 1 --partitions 3