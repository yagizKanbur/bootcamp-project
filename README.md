# Bootcamp Bitirme Projesi
   
## Project timeline

26.07.2021 - Start 
08.08.201 - Deadline

## Prerequisites
* Docker Engine

## Project Architecture
![Project Architecture](https://github.com/yagizKanbur/bootcamp-project/design.png)

## Quick Start
Clone the repositories

https://github.com/yagizKanbur/basket-microservice-new

https://github.com/yagizKanbur/Basket-Notification-Microservice-New

To run microservices, you should run the commands bellow
```sh
docker-compose up --build
prepare.sh
```
## Services
Ps: If you come across jar related errors try to package projects while skipping tests

### Basket
https://github.com/yagizKanbur/basket-microservice-new

Basket microservice handles all the necessary logic for websites shopping basket.

You can check database at http://localhost:8091
You can check Rest Api at http://localhost:8085/swagger-ui/#/

### Users Has Product (BasketNotification)

https://github.com/yagizKanbur/Basket-Notification-Microservice-New

UsersHasProduct holds data about products and the users that have this products in their shopping baskets.
This service is responsible for noticing price and stock changes and at that time sending messages to notification manager to notify users that has the specific product in their basket.

## What I Learned From This Project

In this project I had the chance to use Spring Framework, Kafka and Docker. While working on the project I read various resources, project design could've been changed, and implementations could be made based on resources bellow. 

## Resources
Project Design

https://medium.com/walmartglobaltech/building-domain-driven-microservices-af688aa1b1b8
<https://medium.com/walmartglobaltech/implementing-cart-service-with-ddd-hexagonal-port-adapter-architecture-part-1-4dab93b3fa9f>
https://martinfowler.com/bliki/AnemicDomainModel.html

Kafka 

https://medium.com/trendyol-tech/how-to-integration-test-on-spring-kafka-producer-cb9d1caf0795
