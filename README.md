# payment-method
Provide payment methods that are available for the customer to pay for video platform service

# Used technologies:
  - spring-boot-starter-web
  - spring-data-jpa
  - H2 database
  - lombok
  
# Database: 

  Database scripts provided here:
  
  - src/main/resources/schema.sql
  - src/main/resources/data.sql
  
# Following are endpoints:

# 1. Get all payment method

     This endpoint will return all the payment methods available. And also filtering on name is provided.
     
     Method GET http://localhost/api/v1.0/configuration/payment-methods?name='some-method-name'
     
# 2. Adding a new payment method

     This endpoint will take json request body and add new payment method in database.
     
     Method POST http://localhost/api/v1.0/configuration/payment-methods


# 3. Updating a payment method

     This endpoint will update the payment method in database by name.
     
     Method PUT http://localhost/api/v1.0/configuration/payment-methods/{name}
