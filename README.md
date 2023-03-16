# Overview
This project contains prototype modules for making a simple product order management system based on micro-service architecture. It based on [Spring](https://spring.io/) framework using Spring Boot, Spring Cloud.

# License
This project is currently available under the [MIT](https://github.com/congcoi123/product-order-services/blob/master/LICENSE) License.

# Installation
You can get the sources:
```
git clone https://github.com/congcoi123/product-order-services.git
```



#### Configuration Service
This service provides configurations for all other services (centralized configuration for all services).  
See more: https://cloud.spring.io/spring-cloud-config/multi/multi__spring_cloud_config_server.html

#### Gateway Service
This service is responsible for mapping requests from a client to the desired service endpoint. It based on [Hystrix](https://github.com/Netflix/Hystrix). 

#### Authentication Service
Authorization Server for all other services which grants tokens for the backend resource services. All other secured services must set jwk uri for endpoint implemented on this service.

#### Monitoring Service
Monitoring an application's health and metrics helps us manage it better, notice unoptimized behavior and get closer to its performance. This especially holds true when we're developing a system with many microservices, where monitoring each service can prove to be crucial when it comes to maintaining our system.

### Feature Services
This directory contains all bussiness services.

#### Administration
Comming soon !

#### Customer
Add or update information about a store's customers, including their addresses and whether they have an active customer account with the store.

#### Logger
Comming soon !

#### Master Data
Comming soon !

#### Notification
Comming soon !

#### Order
Create and update a store's orders. Each order is a record of a complete purchase that includes details of the customer, their cart, and any transactions.

#### Payment
Comming soon !

#### Product
Manage a store's products, which are the individual items and services for sale in the store.

#### Shipment
Comming soon !

#### Inventory
List or update the inventory of a variant's inventory item.Each variant can have one inventory item, and each inventory item can have many locations.Each location can have many inventory items for many variants.



## Documentations
Each service directory contains their own `README` file and `ENDPOINTS` documentation.

> Happy coding !
