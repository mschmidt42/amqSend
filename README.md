# amqSend

send data to ActiveMq

```
java -jar app\build\libs\app-all.jar

java -jar app\build\libs\app-all.jar -c "tcp://mq:61616" -h "JMSType" -v "test.dummy" -q myQueue  data/testfile1.json



```