 # Seapay

 - [Description](#Description)
 - [Installation](#Installation)
 - [Additional Infromations](#)

## Description
 
Seapay is a fintech app consists of 4 different services
  - API gateway
    - API gateway service routes all requests to other services
  - User account
    - User account service takes care of user management: user creation, get user data, etc
  - Wallet
    - Wallet service handles all wallet functionalities: update balance, get balance, create wallet, etc
  - Transaction
    - Transaction service manage all transaction data

The project itself has several modules
 - seapay-api
   - a module that abstracts interface for all services
 - seapay-common
   - a module that groups all common functionalities used by all services
 - seapay-domain
   - the bussiness logic for all services goes here
 - seapay-monolith
   - an entry point of our monolithic app, including all handlers
 - seapay-gateway-service
    - microservice to hold all
 - seapay-transaction-service
 - seapay-user-service
 - seapay-wallet-service
  
## Installation
### For Linux
#### Dependencies
 
- Java (JDK >8) : `sudo apt-get install openjdk-8-jdk`
- PostgreSQL (>10) : `sudo apt-get install postgresql`
- Postman (optional to test the API)

#### How to build

```
make all
```

#### How to run
```
make run
```

## Additional Informations

- If you have an authentication failure in PostgreSQL when you build the application
    - ...
