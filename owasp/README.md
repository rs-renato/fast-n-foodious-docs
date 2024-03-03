# 🍔 Fast & Foodious - OWASP ZAP Report

- [OWASP ZAP Report](#owasp-zap-report)
- [Relatórios por Microserviços](#relatorios-por-microservicos)
  - [MS Produto](#ms-produtos)
  - [MS Pedido](#ms-pedido)
  - [MS Pagamento](#ms-pagamento)
  - [Conclusão](#conclusao)

## Relatórios por Microserviços

### MS Produto

- **Cardapio de produtos**
  ![cardapio de produtos](pgn/a-cardapio-produtos-2024-03-03-report.png)
  [Link para relatório completo](pdf/a-cardapio-produtos-2024-03-03-report.pdf)

### MS Pedido

- **Realizacao do pedido (checkout)**
  ![Realizacao do pedido (checkout)](pgn/b-realizacao-do-pedido-checkout-2024-03-03-report.png)
  [Link para relatório completo](pdf/b-realizacao-do-pedido-checkout-2024-03-03-report.pdf)

### MS Pagamento

- **Geracao do Pagamento**
  ![Geracao do Pagamento](pgn/c-geracao-do-pagamento-2024-03-03-report.png)
  [Link para relatório completo](pdf/c-geracao-do-pagamento-2024-03-03-report.pdf)

  - Este endpoint retorna dados do pagamento referente ao ID do pedido, incluindo o `transacaoId` que sera utilizado para confirmacao do pagamento.

- **Confirmacao do Pagamento:**
  ![Confirmacao do Pagamento](pgn/d-confirmacao-do-pagamento-2024-03-03-report.png)
  [Link para relatório completo](pdf/d-confirmacao-do-pagamento-2024-03-03-report.pdf)

  - Este endpoint confirmara o pagamento do pedido, e ira atualizar o pagamento para `CONFIRMADO = 1` ou `REJEITADO = 2`

## Conclusão

Nenhuma ação/atualização posterior as análises foi necessária, uma vez que não foram encontradas ameaças de risco alto pela ferramenta OWASP ZAP. Portanto, os relatórios foram extraídos apenas uma vez para cada serviço.
