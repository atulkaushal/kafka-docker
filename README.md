# Kafka-docker
Project to run Kafka in docker environment.

# Create a single instance of Kafka:
	
	docker-compose -f single-kafka-docker-compose.yml up

# Commands to test the environment:
Create a topic:
	
	kafka-topics --zookeeper zookeeper:2181 --topic docker-topic --create --partitions 3 --replication-factor 1

List topics:
	
	kafka-topics --zookeeper zookeeper:2181 --list