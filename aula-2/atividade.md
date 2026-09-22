# Atividade - Making History

## Disciplina
Elicitação e Requisitos

## Aula 2

---

## 1. Acompanhar o pedido

### História de usuário

Como usuário do aplicativo de delivery, quero acompanhar o status do meu pedido depois da compra, para saber em que etapa ele está e quando será entregue.

### Critérios de aceitação

**Critério 1**

- **Dado** que o usuário realizou uma compra;
- **Quando** acessar o acompanhamento do pedido;
- **Então** deverá visualizar o status atual do pedido.

**Critério 2**

- **Dado** que o restaurante está preparando o pedido;
- **Quando** o usuário consultar o acompanhamento;
- **Então** deverá visualizar que o pedido está em preparação.

**Critério 3**

- **Dado** que o pedido foi encaminhado para entrega;
- **Quando** o usuário consultar o acompanhamento;
- **Então** deverá visualizar que o pedido está em rota de entrega.

---

## 2. Avisar quando um item estiver indisponível

### História de usuário

Como restaurante, quero informar quando um item do cardápio estiver indisponível, para evitar que os clientes façam pedidos de produtos que não podem ser preparados.

### Critérios de aceitação

**Critério 1**

- **Dado** que um item está cadastrado no cardápio;
- **Quando** o restaurante informar que o item está indisponível;
- **Então** o sistema deverá indicar que o item está indisponível para os clientes.

**Critério 2**

- **Dado** que um item está marcado como indisponível;
- **Quando** o cliente visualizar o cardápio;
- **Então** deverá identificar que o item não está disponível para pedido.

**Critério 3**

- **Dado** que o item voltou a estar disponível;
- **Quando** o restaurante alterar sua disponibilidade;
- **Então** o sistema deverá indicar que o item está disponível novamente para os clientes.

---

## 3. Reportar um problema durante a entrega

### História de usuário

Como entregador, quero reportar um problema durante a entrega, para informar o ocorrido e permitir que a situação seja acompanhada pelo suporte.

### Critérios de aceitação

**Critério 1**

- **Dado** que o entregador está realizando uma entrega;
- **Quando** ocorrer um problema durante o percurso;
- **Então** deverá conseguir acessar a opção para reportar o problema.

**Critério 2**

- **Dado** que o entregador acessou a opção de reportar um problema;
- **Quando** selecionar o tipo de problema ocorrido;
- **Então** o sistema deverá registrar a ocorrência relacionada à entrega.

**Critério 3**

- **Dado** que o entregador informou o problema;
- **Quando** confirmar o envio da ocorrência;
- **Então** o sistema deverá informar que o problema foi registrado.

---

# 4. Priorização usando MoSCoW

As três histórias foram priorizadas utilizando o método MoSCoW.

| Ordem | Prioridade | História de usuário |
|---|---|---|
| 1 | **Must Have** | Acompanhar o pedido |
| 2 | **Must Have** | Avisar quando um item do cardápio estiver indisponível |
| 3 | **Should Have** | Reportar um problema durante a entrega |

### Justificativa

**1. Must Have - Acompanhar o pedido**

É uma funcionalidade essencial para que o usuário consiga acompanhar o andamento da compra após realizar o pedido.

**2. Must Have - Avisar quando um item estiver indisponível**

É importante para evitar que os clientes façam pedidos de itens que o restaurante não consegue fornecer.

**3. Should Have - Reportar um problema durante a entrega**

É uma funcionalidade importante para registrar problemas que podem acontecer durante a entrega e permitir que a situação seja comunicada ao suporte.
