# 🍔 Fast & Foodious - OWASP ZAP Report

- [OWASP ZAP Report](#owasp-zap-report)
- [Relatórios por Microserviços](#relatorios-por-microservicos)
  - [MS Produto](#ms-produtos)
  - [MS Pedido](#ms-pedido)
  - [MS Pagamento](#ms-pagamento)
  - [Conclusão](#conclusao)

## Relatórios por Microserviços

### MS Produto

- **Cardapio de produtos:** [GET - http://localhost:3000/v1/produto/categoria/{categoriaId}](pdf/a-cardapio-produtos-2024-03-02-report.pdf)

### MS Pedido

- **Realizacao do pedido (checkout):** [POST - http://localhost:3001/v1/pedido/checkout/{pedidoId}](pdf/b-realizacao-do-pedido-checkout-2024-03-02-report.pdf)

### MS Pagamento

- **Geracao do Pagamento:** [GET - http://localhost:3002/v1/pagamento/{pedidoId}](pdf/c-geracao-do-pagamento-2024-03-02-report.pdf)
  - Este endpoint retorna dados do pagamento referente ao ID do pedido, incluindo o `transacaoId` que sera utilizado para confirmacao do pagamento.
- **Confirmacao do Pagamento:** [POST - http://localhost:3002/v1/pagamento/{transacaoId}/{estadoPagamento}](pdf/d-confirmacao-do-pagamento-2024-03-02-report.pdf)
  - Este endpoint confirmara o pagamento do pedido, e ira atualizar o pagamento para `CONFIRMADO = 1` ou `REJEITADO = 2`

## Conclusão

Nenhuma ação/atualização foi necessária, uma vez que não foram encontradas ameaças de risco alto pela ferramenta OWASP ZAP.
