# Workflow-Livraria--AWS-Step-Functions

## Descrição
Este workflow automatiza o processamento de pedidos na Bellwood Papelaria utilizando **AWS Step Functions** e **AWS Lambda**.

### Fluxo
VerificarEstoque (Lambda) – Checa se o livro está disponível. 
DynamoDB GetItem (Livros) – Busca os detalhes do livro no banco. 
EscolherAção (Choice) – Decide o próximo passo com base na disponibilidade do livro. 
Regra 1: ProcessarPagamento → AtualizarEstoque → Fim 
Regra 2: NotificarFaltaEstoque → NotificarCliente → Fim 

### Tecnologias
- AWS Step Functions  
- AWS Lambda (Node.js/Python)  
- Amazon DynamoDB  
- Amazon SNS (para notificações)

<img width="544" height="668" alt="Image" src="https://github.com/user-attachments/assets/6c7165fc-fb6e-4c91-a445-e9d8e02974b3" />
