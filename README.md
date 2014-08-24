flume-ng-kafka-sink
================

This project is used for [flume-ng](https://github.com/apache/flume) to communicate with [kafka 0.8.1.1].

Configuration of Kafka Sink
----------

    agent_log.sinks.kafka.type = org.apache.flume.sink.kafka.KafkaSink
    agent_log.sinks.kafka.channel = all_channel
    agent_log.sinks.kafka.zk.connect = 127.0.0.1:2181
    agent_log.sinks.kafka.metadata.broker.list = 127.0.0.1:9092
    agent_log.sinks.kafka.topic = all
    agent_log.sinks.kafka.batch.num.messages = 200
    agent_log.sinks.kafka.producer.type = async
    agent_log.sinks.kafka.serializer.class = kafka.serializer.DefaultEncoder
    agent_log.sinks.kafka.request.required.acks = 1

