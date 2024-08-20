//colocar data de registro em cliente

# 1CORRE.API.CLIENTE

## CREATE CLIENTE

### CREATE CLIENTE REQUEST

```js
POST /cliente
```

```json
{
    "nome": "Reinaldo Carlos Castro Alvez",
    "data_nasc": "2001-08-08",
    "cpf": "07512342209",
    "rg": "00011122233",
    "senha": "depoisColocoMaisSeguro",
    "usuario": "Reinaldo Carlos",
    "email": "reinaldaoPequis@gmail.com",
    "telefones": [
        "73998670247", "73998670260"
    ],
    "Endereco": {
        "Estado": "Bahia",
        "Cidade": "Eunápolis",
        "Bairro": "Juca Rosa"
    }
}
```

### CREATE CLIENTE RESPONSE

```js
201 Created
```

```yml
Location: {{host}}/cliente/{id}
```

```json
{
    "id": 0,
    "nome": "Reinaldo Carlos Castro Alvez",
    "data_nasc": "2001-08-08",
    "cpf": "07512342209",
    "rg": "00011122233",
    "data_regis": "2024-09-09",
    "usuario": "Reinaldo Carlos",
    "email": "reinaldaoPequis@gmail.com",
    "telefones": [
        "73998670247", "73998670260"
    ],
    "Endereco": {
        "Estado": "Bahia",
        "Cidade": "Eunápolis",
        "Bairro": "Juca Rosa"
    }
}
```

## GET CLIENTE

### GET CLIENTE REQUEST

```js
GET /cliente/{id}
```

### GET CLIENTE RESPONSE

```js
200 Ok
```

```json
{
    "id": 0,
    "nome": "Reinaldo Carlos Castro Alvez",
    "data_nasc": "2001-08-08",
    "cpf": "07512342209",
    "rg": "00011122233",
    "data_regis": "2024-09-09",
    "usuario": "Reinaldo Carlos",
    "email": "reinaldaoPequis@gmail.com",
    "telefones": [
        "73998670247", "73998670260"
    ],
    "Endereco": {
        "Estado": "Bahia",
        "Cidade": "Eunápolis",
        "Bairro": "Juca Rosa"
    }
}
```

## UPDATE CLIENTE

### UPDATE CLIENTE REQUEST

```js
PUT /cliente/{{id}}
```
```json
{
    "id": 0,
    "nome": "Reinaldo Carlos Castro Alvez",
    "data_nasc": "2001-08-08",
    "cpf": "07512342209",
    "rg": "00011122233",
    "data_regis": "2024-09-09",
    "usuario": "Reinaldo Carlos",
    "email": "reinaldaoPequis@gmail.com",
    "telefones": [
        "73998670247", "73998670260"
    ],
    "Endereco": {
        "Estado": "Bahia",
        "Cidade": "Eunápolis",
        "Bairro": "Juca Rosa"
    }
}
```

### UPDATE CLIENTE RESPONSE

```js
204 No Content
```

ou

```js
201 Created
```
```json
{
    "id": 0,
    "nome": "Reinaldo Carlos Castro Alvez",
    "data_nasc": "2001-08-08",
    "cpf": "07512342209",
    "rg": "00011122233",
    "data_regis": "2024-09-09",
    "usuario": "Reinaldo Carlos",
    "email": "reinaldaoPequis@gmail.com",
    "telefones": [
        "73998670247", "73998670260"
    ],
    "Endereco": {
        "Estado": "Bahia",
        "Cidade": "Eunápolis",
        "Bairro": "Juca Rosa"
    }
}
```

```yml
Location: {{host}}/cliente/{id}
```