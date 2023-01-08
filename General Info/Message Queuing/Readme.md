# What is a Message Queue?
A message queue is an asynchronous system that allows data to move between different services and applications.

![](https://d1.awsstatic.com/product-marketing/Messaging/sqs_seo_queue.1dc710b63346bef869ee34b8a9a76abc014fbfc9.png)

The service that sends the message is known as the producer worker, while the service that receives and responds to messages is known as the consumer worker. However, workable MQs must be extremely scalable in order to allocate the appropriate resources to the number of messages delivered and received.Depending on their loads, you may scale up or down the number of producer and consumer personnel running. 
<br/>

Your system will execute synchronously if you don’t use a message queue. Even though synchronous programming is designed to be simple, it is not particularly efficient. 
<br/>

## **Example Without MQs**
Take, for example, registering for an online service. When you finish filling out your information and click “Sign up,” the system will send you an email and establish a database record for you. Assume you typed in an incorrect, inaccessible email address. For around 10 seconds, the system will try to send you the activation email again. Before being forwarded to the next page, you must wait at least 10 seconds for the system to finish attempting to send an email as a new user. Isn’t that an unsatisfactory user experience? Waiting is a characteristic of an unreliable system.

## **Using MQs**
When you click the “purchase now” button, data is transferred to shipping and distribution networks, but you don’t have to wait for it. Your order is immediately confirmed, and you generally receive an email confirmation and an order reference. A message queue will transport these various pieces of data to their destinations. It distributes them among systems and services, resulting in a more pleasant user experience and a more stable system.

## MQs should be Persistent
It is important that MQs must be persistent. This indicates that the MQ will keep attempting to deliver to the customer even if it isn’t currently available. It’s possible that this is due to a system outage. Persistent MQs, such as IronMQ, will keep attempting until they obtain confirmation from the customer that the data has been received.
<br/>

There is a middle-man or a message broker required for the MQs, and this is where RabbitMQ comes into the picture.

## What is RabbitMQ?
RabbitMQ is a lightweight message broker, which sends and receives messages. It is one of the most popular open-source message brokers, with tens of thousands of users. To address high-scale and high-availability needs, RabbitMQ may also be implemented in a distributed environment. <br/>

Some of RabbitMQ’s alternatives are Apache Kafka, ActiveMQ, KubeMQ, IBM MQ, ZeroMQ, and much more.

## Major terms of RabbitMQ
- **Producing** is just the act of sending. A producer is a software that transmits messages.
- **Queue** is referred to as a post box. Messages pass between RabbitMQ and your apps, but they can only be kept in queues. A queue is effectively a big message buffer that is often limited by the host’s RAM and disc space.
- **Receiving and consuming** have comparable meanings. A consumer is a software that mostly waits for messages to arrive.