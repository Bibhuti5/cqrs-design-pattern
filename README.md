# cqrs-design-pattern

Please Refer this Youtube video if you are struggling :-https://youtu.be/fzGZPf0FMao?si=V0LHYWO-iOYSzUyh

### CreateProduct Event

```
curl --location 'http://localhost:9191/products' \
--header 'Content-Type: application/json' \
--data '{
    "type": "CreateProduct",
    "product": {
        "name": "Books",
        "description": "KK publication",
        "price": 999
    }
}'
```
### UpdateProduct Event

```
curl --location --request PUT 'http://localhost:9191/products/1' \
--header 'Content-Type: application/json' \
--data '{
    "type": "UpdateProduct",
    "product": {
        "id": 1,
        "name": "Watch",
        "description": "Samsung latest model",
        "price": 58000.0
    }
}'
```
