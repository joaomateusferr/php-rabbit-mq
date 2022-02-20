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

## Tests

Now we can run both scripts. In a terminal, run the consumer / receiver [receive.php](/receive.php) then, run the publisher/sender [send.php](/send.php) in another terminal instance.

How to check the operations left to process in the rabbitmq queue

```
sudo rabbitmqctl list_queues
```

## Additional Information

How RabbitMQ works and basic php examples: https://www.rabbitmq.com/tutorials/tutorial-one-php.html

How to install RabbitMQ on Ubuntu through PackageCloud: https://www.rabbitmq.com/install-debian.html#apt-packagecloud