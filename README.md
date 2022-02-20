# How to install RabbitMQ and test with PHP

## Official Repositorys
Take a look at the official RabbitMQ repositorys:

https://github.com/rabbitmq/rabbitmq-server

https://github.com/php-amqplib/php-amqplib

## How Install RabbitMQ On Ubuntu
Take a look at [install_rabbitmq.sh](/install_rabbitmq.sh)

Check if RabbitMQ is active

```
sudo systemctl status  rabbitmq-server.service
```
## Install dependencies to use RabbitMQ with PHP
Just run the following command in the project root

```
sudo composer require php-amqplib/php-amqplib
```

## Test

Now we can run both scripts. In a terminal, run the consumer / receiver (receive.php) then, run the publisher/sender (send.php) in another terminal instance.


```
sudo rabbitmqctl list_queues
```