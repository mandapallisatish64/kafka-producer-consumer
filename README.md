# kafka-producer-consumer

# kafka-commands
#### .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
This command is used to start the zookeeper.Zookeeper is distrubuted management tool which will manage all the kafka brokers.
#### .\bin\windows\kafka-server-start.bat .\config\server.properties
This command is used to run the kafka service by using the properities file.
#### .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic test
This command is used to create topic called test. Topic is a place where kafka will store all the content.
#### java -cp target/kafka-producer-consumer-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.authors.ProducerAuthors test
This will start producer in which we can produce different book authors.
#### java -cp target/kafka-producer-consumer-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.authors.ConsumerAuthors test group1
This is a consumer who wants to consume all the data produced by producer and prints in reverse order.

