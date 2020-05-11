## Endpoint
---

- lista todos veículos
`https://5e1f3d7d39f7a80014a5a349.mockapi.io/api/v1/vehicle`

- lista 10 itens da primeira página

`https://5e1f3d7d39f7a80014a5a349.mockapi.io/api/v1/vehicle?page=1&limit=10`

- lista os itens com status active
`https://5e1f3d7d39f7a80014a5a349.mockapi.io/api/v1/vehicle?filter=false`

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