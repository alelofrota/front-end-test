## Endpoint
---

- listar todos veículos:

`https://5eb9ba733f97140016992030.mockapi.io/vehicle/vehicle`

- listar 10 itens da primeira página:

`https://5eb9ba733f97140016992030.mockapi.io/vehicle?page=1&limit=10`

- Buscar um veiculo pelo numero da placa:

`https://5eb9ba733f97140016992030.mockapi.io/vehicle?filter=ABC-4852`

- lista os itens com status active:

`https://5eb9ba733f97140016992030.mockapi.io/vehicle?filter=true`


##### Objeto retornado pela API

```json
{
  "id": "1",
  "plate": "ABC-1 ",
  "model": "Class C 1.1 Avantgarde Turbo Flex ",
  "manufacturer": "Mercedes-Benz",
  "color": "black",
  "status": true
}
``` 

### Métodos

`[GET] /vehicle` Lista todos veículos

`[GET] /vehicle/:id` Retorna um veículo específico

`[POST] /vehicle` Cria um novo veículo

`[PUT] /vehicle/:id` Atualiza um veículo

`[DELETE] /vehicle/:id` Remove um veículo