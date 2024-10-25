Desafio: Refinando um Projeto de Banco de Dados - E-COMMERCE

Objetivo:
Refine o modelo apresentado acrescentando os seguintes pontos:

Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
Entrega – Possui status e código de rastreio;

Solução: 
Cliente PJ e PF – Na entidade cliente foi adicionado os campos: CPNJ/CPF,Email e tipo (EMUM Pessoa Júridica ou Pessoa Física) item CPNJ/CPF e Email como (UNIQUE)
Pagamento - Criada a entidade PAGAMENTO com Informaçoes do cartão de Crédito (Nome,número do cartão e validade), com Relacionamento 1,N com entidade CLIENTE.
Entrega – Na entidadde Pedido foi adionado os campos ( ENTREGUE como tipagem ENUM SIM/NÂO e CÓDIGO DE RASTREIO). com relacionamento 1,N com Entidade CLIENTE.

![image](https://github.com/user-attachments/assets/e6953263-8784-4b7e-a0f1-babb18d0f8d1)

