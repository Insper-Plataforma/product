# Estrutura de pastas

```bash
src/main/java/store/product/
├── ProductController.java  # Interface Feign
├── ProductIn.java          # DTO de entrada
└── ProductOut.java         # DTO de saída
```

## ProductIn

Representa os dados de entrada para cadastro de produto.

```java
record ProductIn(
    String name,
    Double price,
    String unit
)
```

- `name`: nome do produto

- `price`: preço unitário

- `unit`: unidade de medida (ex: kg, un, L)

---

## ProductOut

Representa a resposta da API ao lidar com produtos.

```java
record ProductOut(
    String id,
    String name,
    Double price,
    String unit
)
```

- `id`: identificador único do produto
- `name`: nome do produto
- `price`: preço unitário
- `unit`: unidade de medida (ex: kg, un, L)
