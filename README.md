# amqSend

send data to ActiveMq

```
java -jar app\build\libs\app-all.jar

java -jar app\build\libs\app-all.jar -c "tcp://mq:61616" -h "JMSType" -v "test.dummy" -q myQueue  data/testfile1.json


```

Help:
```
Usage: amqSend [-r] [-c=<connectionUrl>] [-h=<headerName>] [-q=<queueName>]
               [-v=<headerValue>] <file>
Sends a message to ActiveMQ
      <file>                A (JSOM) file containing the date to send as text
  -c, --connection=<connectionUrl>
                            the conection to use. Default: "tcp://localhost:
                              61616"
  -h, --header-name=<headerName>
                            the header name to send. Default: "JMSType"
  -q, --queue=<queueName>   The destinantion queue.
  -r, --remove-nl           remove \n, \r and \t characters.
  -v, --header-value=<headerValue>
                            the header value to send. Default: "unknown"
```

Used Libraries:
* activemq-client
* picocli
