Trabalho DM107
=============
 **Tipo de Autenticação**: Para ambas as API's Basic Auth, senha e Usuário são "admin"<br>
 
**Media type consumido**: contentType/Json
**Media type produzido**: contentType/Json

**Endpoint's**
**Java**:
 1. Metodo -> GET -> http://localhost:8081/trabalho_dm107/rest/apiEntrega/numeroPedido/{id}
  
- Traz as informações da Entrega.

2. Metodo -> POST -> http://localhost:8081/trabalho_dm107/rest/apiEntrega/numeroPedido/
 
 - Insere uma nova entrega nos registro.
 
 Parâmetros:
 
 ```
 { 
  "numeroPedido": Int,
  "idCliente": Int, 
  "nomeRecebedor": String, 
  "cpfRecebedor": String, 
  "dataEntrega": String 
 }
```
Php:

1. Metodo -> GET -> http://localhost/DM107/TrabalhoDM107/src/public/entrega/numeroPedido/{id}
- Traz a entrega pelo numero do pedido.
2. Metodo -> PUT -> http://localhost/DM107/TrabalhoDM107/src/public/entrega/{id}
- Altera as informações da entrega.
Parâmentros:
```
{
 "numero_pedido": Long,
 "id_cliente": Long,
 "nome_recebedor":string,
 "cpf_recebedor": string ,
 "data_entrega": "YYYY-mm-dd"
}
  ```
3. Metodo -> DELETE -> http://localhost/DM107/TrabalhoDM107/src/public/entrega/delete/{id}
- Deleta uma entrega pelo ID;

**Status**:
- 200: Success	
- 401:Unauthorized	
- 500: Internal Server Erro	
