# 03 - Starting With The Backend

<br/>

```
$ npm install nodemon express dotenv morgan mongoose corse
$ npm start
```

<br/>

GET -> http://localhost:3000/api/v1/products/

<br/>

```
$ docker-compose up
```

<br/>

```
Compas

Create Database:
database name: eshop-database
collection name: products
```

<br/>

```
// POST
$ curl \
    --data '{
      "id":"1",
      "name":"hair dresser",
      "image":"image_url",
      "countInStock": 500}' \
    --header "Content-Type: application/json" \
    --request POST \
    --url http://localhost:3000/api/v1/products \
    | jq
```

<br/>

**response:**

```
{
  "name": "hair dresser",
  "image": "image_url",
  "countInStock": 500,
  "_id": "646d0e5954d09a11f1292510",
  "__v": 0
}
```

<br/>

```
// GET
$ curl \
    --header "Content-Type: application/json" \
    --request GET \
    --url http://localhost:3000/api/v1/products \
    | jq
```

<br/>

---

<br/>

**Marley**

Any questions in english: <a href="https://jsdev.org/chat/">Telegram Chat</a>  
Любые вопросы на русском: <a href="https://jsdev.ru/chat/">Телеграм чат</a>
