# Interface Product

A interface `ProductController` define os contratos REST expostos pelo `product-service`.

Ela funciona como um **Feign Client** e permite:

- Criar novos produtos
- Listar produtos
- Buscar produto por ID
- Excluir um produto

Esta interface deve ser implementada por um microsserviço com persistência (como o `product-service`).

---