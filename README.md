# Cars API
This application is built using spring-boot and hosts three microservices. The cars API is build upon consumption of these services through eureka server.

## Background
The features include
1. We have a map service boogle-maps, registered in the eureka server, which provides address of a location
2. We have a pricing service, registered in the eureka server, which provides price of a vehicle 
3. Vehicles API, which consumes above services and lets us perform CRUD operation on cars.

## How To Run
1. Have Java 1.8 installed
2. Have maven package installed
3. Clone the repository first
    ```$cmd
    git clone https://github.com/debatanu-thakur/car-api.git
    ```
4. Make sure http://localhost:8080, 8761, 8082 and 9191 is available
5. Run using command, under each service folder
    ```
    mvn spring-boot:run
    ```
   Or
   
   Under the root folder
   ```
   docker-compse up
   ```
6. To test, you have to go into `pricing-service` and `vehicles-api` folder and run `mvn test`
### License
MIT