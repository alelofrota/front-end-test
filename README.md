# Front End Test

## Objetivo

Criar uma app "To-do list" utilizando Angular 7+ integrando com os endpoints abaixo.

A app deve utilizar rotas, componentes e ter uma tela para cada função.

Deverá ter as opções:

- Listar as categorias
- Listar e inserir listas
- Listar, inserir itens e marcar como "feito"

## Endpoint

`http(s)://5e1f3d7d39f7a80014a5a349.mockapi.io/api/v1/`

## Categories

```json
{
  "id": "ID da categoria (Gerado)",
  "name": "Nome da categoria"
}
``` 

`[GET] /categories` Lista categorias

`[GET] /categories/:id` Retorna uma categoria específica

`[POST] /categories` Insere uma categoria

`[PUT] /categories/:id` Atualiza uma categoria

`[DELETE] /categories/:id` Remove uma categoria

## Lists

```json
{
  "id": "ID da lista (Gerado)",
  "name": "Nome da lista"
}
``` 

`[GET] /categories/:idCategory/lists` Lista as listas de uma categoria

`[GET] /categories/:idCategory/lists/:id` Retorna uma lista específica de uma categoria

`[POST] /categories/:idCategory/lists` Insere uma lista em uma categoria

`[PUT] /categories/:idCategory/lists/:id` Atualiza uma lista de uma categoria

`[DELETE] /categories/:idCategory/lists/:id` Remove uma lista de categoria

## Items

```json
{
  "id": "ID do item (Gerado)",
  "name": "Nome do item",
  "done": true,
}
``` 

`[GET] /categories/:idCategory/lists/:idList/items` Lista os itens de uma lista

`[GET] /categories/:idCategory/lists/:idList/items/:id` Retorna um item

`[POST] /categories/:idCategory/lists/:idList/items` Insere um item em uma lista

`[PUT] /categories/:idCategory/lists/:idList/items/:id` Atualiza um item da lista

`[DELETE] /categories/:idCategory/lists/:idList/items/:id` Remove um item

