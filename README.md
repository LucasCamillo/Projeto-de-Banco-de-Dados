# Banco de Dados - E-commerce de Roupas Destiny Chronicles

Este repositório contém o modelo de banco de dados utilizado para um projeto acadêmico voltado à criação de uma loja virtual especializada em roupas com temáticas mitológicas (grega, nórdica, egípcia, japonesa, entre outras).

## 📘 Descrição

O objetivo principal deste banco de dados é estruturar as informações necessárias para o funcionamento básico de um e-commerce, incluindo o cadastro de clientes, controle de pedidos, pagamentos, entregas, produtos e estoque.

Este projeto foi desenvolvido como parte de um trabalho universitário na disciplina de modelagem de banco de dados e também representa a fase inicial de um projeto pessoal de marca de moda autoral.

##  Estrutura do Banco

O banco foi implementado em **MySQL**, e conta com as seguintes tabelas:

- `CLIENTE` – Armazena dados dos clientes.
- `PRODUTO` – Contém as informações dos produtos (camisetas, moletons, jaquetas, etc).
- `ESTOQUE` – Controla a quantidade disponível de cada produto.
- `PEDIDO` – Registra os pedidos realizados.
- `ITEM_PEDIDO` – Detalha os produtos incluídos em cada pedido.
- `PAGAMENTO` – Registra as informações de pagamento.
- `ENTREGA` – Armazena os dados de rastreamento de entrega.

###  Relacionamentos principais

- Um cliente pode fazer vários pedidos.
- Cada pedido possui **um** pagamento e **uma** entrega associada.
- Um pedido pode conter **vários produtos**, e um produto pode estar em **vários pedidos** (relacionamento N:N através de `ITEM_PEDIDO`).
