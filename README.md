## CRUD - SpringBoot
Starting SpringBoot with CRUD requests.   
(amigoscode classes)

### Prerequisites
* PostgreSQL
* Docker
  ``start before running``

### Post
````
curl --location --request GET 'localhost:8080/api/v1/customers' \
--header 'Content-Type: application/json' \
--data-raw '{
"name": "vitor",
"email": "vitor@gmail.com",
"age": 33
}'
````

### Get (all)
````
curl --location 'localhost:8080/api/v1/customers'
````

### Delete (by ID)
````
curl --location --request DELETE 'localhost:8080/api/v1/customers/1'
````

### Put (update by ID)
````
curl --location --request PUT 'localhost:8080/api/v1/customers/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "vitor",
    "email": "vitorAtualizado@gmail.com",
    "age": 33
}'
````
