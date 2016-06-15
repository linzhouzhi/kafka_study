# kafka_study
* 新建工程
mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=kafka_demo
* 开启kafka broker
bin/kafka-server-start.sh config/server-1.properties &
bin/kafka-server-start.sh config/server-2.properties &
* 创建topic
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 3 --partitions 1 --topic my-replicated-topic
* 运行producer
* 运行consumer
