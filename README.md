### Spring Boot PACT test demo

A simple Spring Boot application, demonstrating implementation of contract testing using PACT testing framework.

## Usage

Instance of PACT broker can be deployed using provided `docker-compose.yaml` file. 

To start up PACT broker make sure you have docker installed. Then call `docker compose up` from terminal.

Both consumer and provider implement a simple RESTapi demonstrating a full configuration and implementation of a contract testing in two Spring Boot application.

To start tests in consumer call `gradle clean test pactPublish` to run tests and publish contract to the Pact broker. Make sure Pact broker is running and host name is configured correctly in `build.gradle`.

In provider simple `gradle clean test` will do. No need to publish contract as you've done so in consumer.