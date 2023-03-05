![download](https://user-images.githubusercontent.com/34875169/169837256-b5cce5b4-0b10-4a5b-82b7-926f10690437.png)
***
How to setup confluent Kafka.
1. [Account Setup](Confluent%20Account.md)
2. [Cluster Setup](ConfluentClusterSetup.md)
3. [Kafka Topic](Confluent%20Topic%20Creation.md)
4. [Obtain Cloud secrets](Kafka%20key%20and%20secrets.md)
5. [Obtain Schema secrets](SchemaRegistry.md)
***

Create a conda environment
```
conda create -p venv python==3.8 -y
```

Activate conda environment
```
conda activate venv
```

To use confluent kafka we need following details from Confluent dashboard.

```
confluentClusterName = ""
confluentBootstrapServers = ""
confluentTopicName = ""
confluentApiKey = ""
confluentSecret = ""
```
Add below library in requirements.txt
```
confluent-kafka[avro,json,protobuf]
pyspark==3.2.1
```