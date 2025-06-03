# Endpoints - Feign Interface `ProductController`

Todos os endpoints se referem ao microsserviço `product` com base URL: `http://product:8080`.

---

### POST `/product`

Cria um novo produto.

- **Request body**: [`ProductIn`](./entidades.md#productin)
- **Response**: [`ProductOut`](./entidades.md#productout)

---

### GET `/product`

Retorna todos os produtos cadastrados.

- **Response**: `List<ProductOut>`

---

### GET `/product/{idProduct}`

Busca um produto pelo seu ID.

- **Path param**: `idProduct`
- **Response**: [`ProductOut`](./entidades.md#productout)

---

### DELETE `/product/{idProduct}`

Remove um produto do sistema.

- **Path param**: `idProduct`
- **Response**: `204 No Content`
