<h1 align="center">Fundamentos do NodeJS</h1>

## Métodos de requisição HTTP

- **GET:** Buscar uma informação no servidor;
- **POST:** Inserir uma informação no servidor;
- **PUT:** Alterar uma informação no servidor;
- **PATCH:** Alterar uma informação específica;
- **DELETE:** Deletar uma informação no servidor.

## Tipos de Parâmetros

### Route Params

Eles são passados diretamente na rota e são usados para buscar, identificar, editar e excluir um recurso, sem eles a
rota não funciona.

Exemplo:

```
GET http://localhost:3333/courses/1
```

### Query Params

Eles também estão presentes na rota, mas além de não serem obrigatórios para que a rota funcione, são mais utilizados
para paginação e filtros.

Exemplo:

```
GET http://localhost:3333/courses?page=1&order=asc
```

### Body Params

São utilizados para a inserção ou alteração de um recurso, ou seja, no momento do cadastro e atualização dos dados.

```
POST
{
 "name": "Matheus",
 "age": 24,
 "email": "matheusmoreira.g6@gmail.com"
}
```
