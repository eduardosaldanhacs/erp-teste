# erp-teste
✅ Banco de Dados:
Criação de 4 tabelas principais: pedidos, produtos, cupons, estoque

✅ Cadastro de Produtos:
Tela com formulário para cadastrar:
Nome
Preço
Variações
Estoque

Cada variação possui controle individual de estoque (funcionalidade bônus implementada)
Associação automática entre os produtos e seus respectivos estoques

✅ Atualização:
Permite editar os dados do produto e atualizar o estoque diretamente na mesma tela

✅ Carrinho de Compras com Sessão:
Botão "Comprar" para adicionar produtos ao carrinho
Gerenciamento do carrinho via $_SESSION, com controle de quantidade e estoque disponível
Cálculo automático de frete com regras:
Subtotal entre R$52,00 e R$166,59 → Frete R$15,00
Subtotal acima de R$200,00 → Frete grátis
Outros valores → Frete R$20,00

✅ Consulta de CEP:
Integração com ViaCEP para preenchimento automático do endereço
Funcionalidades Adicionais

✅ Cupons de Desconto:
Cadastro e validação de cupons com:
Data de validade
Valor mínimo baseado no subtotal do pedido

✅ Envio de E-mail:
Após finalizar o pedido, é enviado um e-mail de confirmação com os dados do endereço preenchido

✅ Webhook de Status de Pedido:
Recebe o ID do pedido e o status via endpoint
Se status = cancelado, o pedido é removido
Para outros status, o pedido é atualizado
