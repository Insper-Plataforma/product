# Setup e Execução - Interface Product

Este módulo define os contratos da API REST do serviço de produtos.

---

## Requisitos

- Java 17+
- Spring Boot
- Lombok
- OpenFeign

---

## Dependências no `pom.xml`

- `spring-boot-starter-web`
- `spring-cloud-starter-openfeign`
- `lombok`

---

## Como usar

Este módulo deve ser implementado por um serviço persistente (`product-service`) e pode ser consumido por outros microsserviços que precisam buscar informações de produtos.

### Exemplo de uso via Feign:

```java
@FeignClient(name = "product", url = "http://product:8080")
public interface ProductController {
    // ...
}
```
