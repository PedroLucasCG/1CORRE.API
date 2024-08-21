//Criar o doc para quebras de acordo
# 1CORRE.API.ACORDO

## CREATE ACORDO

### CREATE ACORDO REQUEST

```js
POST /acordo
```

```json
{
    "cliente": 1,
    "oferta": 1,
    "valor": 100.00,
    "estado": 1,
    "descricao": "Contrato firmado de limpeza de terrreno por 10$",
    "modalidade": "fixo"
}
```

### CREATE ACORDO RESPONSE
```js
201 Created
```

```yml
Location: {{host}}/acordo/{id}
```

```json
{
    "id": 0,
    "cliente": 1,
    "oferta": 1,
    "valor": 100.00,
    "estado": 1,
    "descricao": "Contrato firmado de limpeza de terrreno por 10$",
    "modalidade": "fixo"
}
```

## GET ACORDO

### GET ACORDO REQUEST

```js
GET /acordo?cliente=1&oferta=1&estado=1
```

### GET ACORDO RESPONSE

```js
200 Ok
```

```json
{
    "id": 0,
    "cliente": 1,
    "oferta": 1,
    "valor": 100.00,
    "estado": 1,
    "descricao": "Contrato firmado de limpeza de terrreno por 10$",
    "modalidade": "fixo"
}
```

## UPDATE ACORDO

### UPDATE ACORDO REQUEST

```js
GET /acordo/{{id}}
```

```json
{
    "id": 0,
    "cliente": 1,
    "oferta": 1,
    "valor": 100.00,
    "estado": 1,
    "descricao": "Contrato firmado de limpeza de terrreno por 10$",
    "modalidade": "fixo"
}
```

### UPDATE ACORDO RESPONSE

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
    "cliente": 1,
    "oferta": 1,
    "valor": 100.00,
    "estado": 1,
    "descricao": "Contrato firmado de limpeza de terrreno por 10$",
    "modalidade": "fixo"
}
```