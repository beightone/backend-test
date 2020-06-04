# Welcome B8ONE Backend Test!
Hi! We are happy with your willingness to work with us! In short, this test contains a challenge to build a clean api architecture with good pattern and best practices.

## Use

- Typescript (tsc to build aplication in docker workflow)
- NodeJS
- DataFetch (REST or Graphql)
- PostgreSQL
- any ORM

## Goals

- Nice to have a TDD approach.
- Create a good initial code clean boilerplate, folder structure, scalable code and easy readable for other developers.
- A good think in build a scalable architeture.
- Time is not a preference but we like a blood in the eyes people.
- Best practices GraphQL or Rest implementation.
- Structure a good migrations and seeds to local test.
- Docker-compose for we build the project.
- Use best practices in ES.

## Logic Goal

Build a small aplication for avalliate all of this concepts.

## Tables structure

### Order 

* id: string
* order_number: string
* user_id: FK references - user.id (1 - n)
* status: enum('active', 'process', 'closed')

### User

* id: string
* name: string
* lastName?: string
* email: string

### Address

* boulevard
* neighboorhood
* number

### User_Address (n + n)

* id
* user_id: FK references - user.id
* address_id: FK references - user.id
* active: boolean


## You need to build:

- Endpoint to insert a new user.
- Endpoint to insert a new order with user id to relation.
- Endpoint to insert a new address with user to relation.
- endpoint to handle order status
- endpoint to get user with populated active addresses and all orders.
- endpoint to get order with populated user
- endpoint to desactive user address.

**Good Luck** 
