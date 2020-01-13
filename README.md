# Currenncy-Conversion-service
A demonstration project for microservice using following 6 spring boot project:
1. currency-conversion-service
2. currency-exchange-service
3. netflix-eureka-naming-server
4. netflix-zuul-api-gateway-server
5. zipkin-server
6. rabbitmq

# Steps to test the project
1. Download docker-compose.yml
2. Install docker on your system
3. Use terminal and change the directory where the docker-compose.yml file is.
4. Run this command -  docker-compose up 

# Test the rest api provided by the project
1. currency-conversion-service  http://localhost:8100/currency-conversion-feign/from/USD/to/INR/1000    The actual endpoint is http://localhost:8100/currency-conversion-feign/from/{from}/to/{to} with possible values of from= USD,EUR, AUD and to= INR
2. currency-exchange-service    http://localhost:8000/currency-exchange/from/EUR/to/INR
3. netflix-eureka-naming-server http://localhost:8761
4. netflix-zuul-api-gateway-server  
5. zipkin-server                http://localhost:9411
6. rabbitmq                     http://localhost:15672     use guest and guest as the password.

# Technologies used in this project
Spring boot (MVC, Data rest, AOP), feign, ribbon, zuul api gateway, eureka, sleuth, zipkin, rabbitmq

