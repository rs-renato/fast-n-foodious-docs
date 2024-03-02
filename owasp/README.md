# 🍔 Fast & Foodious - OWASP ZAP Report

- [Relatórios por Microserviços](#relatorios-por-microservicos)
  - [MS Produto](#ms-produtos)
  - [MS Pedido](#ms-pedido)
  - [MS Pagamento](#ms-pagamento)
  - [Conclusão](#conclusao)

## Relatórios por Microserviços

### MS Produto

- Cardapio de produtos: `GET - http://localhost:3000/v1/produto/categoria/{categoriaId}`

### MS Pedido

- Realizacao do pedido (checkout): `POST - http://localhost:3001/v1/pedido/checkout/{pedidoId}`

### MS Pagamento

- Geracao do Pagamento: `GET - http://localhost:3002/v1/pagamento/{pedidoId}`
  - Este endpoint retorna dados do pagamento referente ao ID do pedido, incluindo o `transacaoId` que sera utilizado para confirmacao do pagamento.
- Confirmacao do Pagamento: `POST - http://localhost:3002/v1/pagamento/{transacaoId}/{estadoPagamento}`
  - Este endpoint confirmara o pagamento do pedido, e ira atualizar o pagamento para `CONFIRMADO = 1` ou `REJEITADO = 2`

## Conclusão

Nenhuma ação/atualização foi necessária, uma vez que não foram encontradas ameaças de risco alto pela ferramente OWASP ZAP.
