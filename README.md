# Workflow-Livraria--AWS-Step-Functions

## 🪶 Workflow de Pedidos - Bellwood Papelaria

### Descrição
Este workflow automatiza o processamento de pedidos na Bellwood Papelaria utilizando **AWS Step Functions** e **AWS Lambda**.

### Fluxo
1. ReceberPedido → Captura os dados do pedido.
2. VerificarEstoque → Checa disponibilidade no estoque.
3. EscolherAção:
   - Se disponível → ProcessarPagamento → AtualizarEstoque → End
   - Se indisponível → NotificarFaltaEstoque → End

### Tecnologias
- AWS Step Functions  
- AWS Lambda (Node.js/Python)  
- Amazon DynamoDB  
- Amazon SNS (para notificações)
