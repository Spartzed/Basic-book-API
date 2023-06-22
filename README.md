## API documentation

This repository contains the implementation of the My Application API, which provides endpoints to interact with book-related resources in a virtual bookstore.

## Books

#### Return all Books

```http
  GET /api/books
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `jwt-token` | `string` | **Required**. JWT TOKEN |

#### Create a Book

```http
  POST /api/books
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `jwt-token` | `string` | **Required**. JWT TOKEN |
| `name` | `int` | **Required**. Book name |
| `isbn` | `int` | **Required**. Book isbn |
| `value` | `int` | **Required**. Book value |

#### Return a Book

```http
  GET /api/books/{id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `jwt-token` | `string` | **Required**. JWT TOKEN |
| `id`      | `string` | **Required**. Book ID |

#### Update Book

```http
  PUT /api/books/{id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `jwt-token` | `string` | **Required**. JWT TOKEN |
| `id`      | `string` | **Required**. Book ID |

#### Delete a book

```http
  DELETE /api/books/{id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `jwt-token` | `string` | **Required**. JWT TOKEN |
| `id`      | `string` | **Required**. Book ID |


## Authentication

#### Login

```http
  POST /api/login
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `email`      | `string` | **Required**. User email |
| `password`      | `string` | **Required**. User password |

#### Logout

```http
  POST /api/logout
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `jwt-token` | `string` | **Required**. JWT TOKEN |
