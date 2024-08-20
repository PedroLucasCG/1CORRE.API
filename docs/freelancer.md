//adicionar verbo delete

# 1CORRE.API.FREELANCER

## CREATE FREELANCER

### CREATE FREELANCER REQUEST

```js
POST /freelancer;
```

```json
{
  "nome": "Regina Castro Alvez",
  "data_nasc": "2001-08-08",
  "cpf": "07512342209",
  "rg": "00011122233",
  "senha": "depoisColocoMaisSeguro",
  "usuario": "Regina Confeitera",
  "email": "Regina@confeitera.com",
  "telefones": ["73998670247", "73998670260"],
  "Endereco": {
    "Estado": "Bahia",
    "Cidade": "Eunápolis",
    "Bairro": "Pequi"
  },
  "Oferta": [
    { "Confeitaria": null },
    {
      "Salgados": {
        "nome": "Salgados da festa do prefeito",
        "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
        "url": "https://app.jotaja.com/salgados.com"
      }
    }
  ]
}
```

### CREATE FREELANCER RESPONSE

```js
201 Created
```

```yml
Location: {{host}}/freelancer/{id}
```

```json
{
  "id": 0,
  "nome": "Regina Castro Alvez",
  "data_nasc": "2001-08-08",
  "cpf": "07512342209",
  "rg": "00011122233",
  "usuario": "Regina Confeitera",
  "email": "Regina@confeitera.com",
  "data_regis": "2025-05-09",
  "telefones": ["73998670247", "73998670260"],
  "Endereco": {
    "Estado": "Bahia",
    "Cidade": "Eunápolis",
    "Bairro": "Pequi"
  },
  "Oferta": [
    { "Confeitaria": null },
    {
      "Salgados": {
        "nome": "Salgados da festa do prefeito",
        "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
        "url": "https://app.jotaja.com/salgados.com"
      }
    }
  ]
}
```

## GET FREELANCER

### GET FREELANCER REQUEST

```js
GET /freelancer?data_resgis={{data_regis}}&oferta={{oferta1}},{{oferta2}}
```

### GET FREELANCER RESPONSE

```js
200 Ok
```

```json
//Retorna um array com todos os valores que correspondem a pesquisa
{
    [
        {
        "id": 0,
        "nome": "Regina Castro Alvez",
        "data_nasc": "2001-08-08",
        "cpf": "07512342209",
        "rg": "00011122233",
        "usuario": "Regina Confeitera",
        "email": "Regina@confeitera.com",
        "data_regis": "2025-05-09",
        "telefones": ["73998670247", "73998670260"],
        "Endereco": {
            "Estado": "Bahia",
            "Cidade": "Eunápolis",
            "Bairro": "Pequi"
        },
        "Oferta": [
            { "Confeitaria": null },
            {
            "Salgados": {
                "nome": "Salgados da festa do prefeito",
                "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
                "url": "https://app.jotaja.com/salgados.com"
            }
            }
        ]
        }
    ]
}
```

## GET FREELANCER SIMPLE

### GET FREELANCER SIMPLE REQUEST

```js
GET /freelancer?data_resgis={{data_regis}}&oferta={{oferta1}},{{oferta2}}

```

### GET FREELANCER SIMPLE RESPONSE

```js
200 Ok
```

```json
//Retorna um array com todos os valores que correspondem a pesquisa
{
    [
        {
        "id": 0,
        "usuario": "Regina Confeitera",
        "email": "Regina@confeitera.com",
        "telefones": [
            "73998670247", "73998670260"
        ],
        "Endereco": {
            "Estado": "Bahia",
            "Cidade": "Eunápolis",
            "Bairro": "Pequi"
        },
        "Oferta": [
            {"Confeitaria": null},
            {
                "Salgados": {
                    "nome": "Salgados da festa do prefeito",
                    "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
                    "url": "https://app.jotaja.com/salgados.com"
                }
            }
        ]
        }
    ]
}

```

## UPDATE FREELANCER

### UPDATE FREELANCER REQUEST

```js
PUT /freelancer/{{id}}
```

```json
{
  "nome": "Regina Castro Alvez",
  "data_nasc": "2001-08-08",
  "cpf": "07512342209",
  "rg": "00011122233",
  "senha": "depoisColocoMaisSeguro",
  "usuario": "Regina Confeitera",
  "email": "Regina@confeitera.com",
  "telefones": ["73998670247", "73998670260"],
  "Endereco": {
    "Estado": "Bahia",
    "Cidade": "Eunápolis",
    "Bairro": "Pequi"
  },
  "Oferta": [
    { "Confeitaria": null },
    {
      "Salgados": {
        "nome": "Salgados da festa do prefeito",
        "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
        "url": "https://app.jotaja.com/salgados.com"
      }
    }
  ]
}
```

### UPDATE FREELANCER RESPONSE

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
  "nome": "Regina Castro Alvez",
  "data_nasc": "2001-08-08",
  "cpf": "07512342209",
  "rg": "00011122233",
  "usuario": "Regina Confeitera",
  "email": "Regina@confeitera.com",
  "data_regis": "2025-05-09",
  "telefones": ["73998670247", "73998670260"],
  "Endereco": {
    "Estado": "Bahia",
    "Cidade": "Eunápolis",
    "Bairro": "Pequi"
  },
  "Oferta": [
    { "Confeitaria": null },
    {
      "Salgados": {
        "nome": "Salgados da festa do prefeito",
        "descricao": "Nesta página consta os links dos salgados feitos para a festa do prefeito!!!",
        "url": "https://app.jotaja.com/salgados.com"
      }
    }
  ]
}
```

```yml
Location: {{host}}/freelancer/{{id}}
```

## DELETE FREELANCER

### DELETE FREELANCER REQUEST

```js
DELETE /freelancer/{{id}}
```

### DELETE FREELANCER RESPONSE

```js
204 No Content
```
