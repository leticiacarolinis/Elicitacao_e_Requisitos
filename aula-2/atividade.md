# Atividade - Making History

## Disciplina
Elicitação e Requisitos

## Aula
Aula 2

---

## 1. Acompanhar o pedido

### História de usuário

**Como usuário do aplicativo de delivery, quero acompanhar o status do meu pedido após a compra, para saber em que etapa ele está e quando será entregue.**

### Critérios de aceitação

**Critério 1**

- **Dado** que o usuário realizou um pedido;
- **Quando** acessar a área de acompanhamento do pedido;
- **Então** deverá visualizar o status atual do pedido.

**Critério 2**

- **Dado** que o pedido está sendo preparado pelo restaurante;
- **Quando** o usuário consultar o acompanhamento;
- **Então** deverá visualizar que o pedido está em preparação.

**Critério 3**

- **Dado** que o pedido foi enviado para entrega;
- **Quando** o usuário acessar o acompanhamento;
- **Então** deverá visualizar que o pedido está em rota de entrega.

---

## 2. Avisar sobre item indisponível

### História de usuário

**Como restaurante, quero informar quando um item do cardápio estiver indisponível, para evitar que clientes façam pedidos de produtos que não podem ser preparados.**

### Critérios de aceitação

**Critério 1**

- **Dado** que um item está cadastrado no cardápio;
- **Quando** o restaurante alterar sua disponibilidade para indisponível;
- **Então** o item deverá ser identificado como indisponível para os clientes.

**Critério 2**

- **Dado** que um item está marcado como indisponível;
- **Quando** um cliente visualizar o cardápio;
- **Então** deverá saber que o item não pode ser pedido.

**Critério 3**

- **Dado** que o item voltou a estar disponível;
- **Quando** o restaurante alterar seu status para disponível;
- **Então** o item deverá voltar a aparecer como disponível para os clientes.

---

## 3. Reportar problema durante a entrega

### História de usuário

**Como entregador, quero reportar um problema durante a entrega, para informar a situação e permitir que o restaurante ou o suporte tome as providências necessárias.**

### Critérios de aceitação

**Critério 1**

- **Dado** que o entregador está realizando uma entrega;
- **Quando** ocorrer um problema durante o percurso;
- **Então** deverá conseguir acessar a opção para reportar o problema.

**Critério 2**

- **Dado** que o entregador acessou a opção de reportar problema;
- **Quando** selecionar o tipo de problema ocorrido;
- **Então** o sistema deverá registrar a ocorrência relacionada à entrega.

**Critério 3**

- **Dado** que o problema foi registrado;
- **Quando** o entregador confirmar o envio da ocorrência;
- **Então** o sistema deverá informar que o problema foi registrado com sucesso.

---

# 4. Priorização utilizando MoSCoW

As necessidades foram organizadas utilizando o método MoSCoW, que classifica as funcionalidades de acordo com sua prioridade.

| Prioridade | Necessidade | Justificativa |
|---|---|---|
| **Must Have** | Acompanhar o pedido | É uma funcionalidade essencial para que o cliente tenha informações sobre o andamento do pedido após a compra. |
| **Must Have** | Avisar sobre item indisponível | Evita que pedidos sejam realizados com produtos que o restaurante não possui, reduzindo problemas no atendimento. |
| **Should Have** | Reportar problema durante a entrega | É importante para registrar ocorrências e permitir que problemas durante a entrega sejam comunicados. |

### Ordem de prioridade

1. **Must Have - Acompanhar o pedido**
2. **Must Have - Avisar sobre item indisponível**
3. **Should Have - Reportar problema durante a entrega**

As três funcionalidades são relevantes para o aplicativo, porém as duas primeiras foram consideradas essenciais para o funcionamento básico do processo de compra e atendimento. O reporte de problemas durante a entrega foi classificado como Should Have por ser uma funcionalidade importante de suporte ao processo.

---

## 5. INVEST

As histórias foram elaboradas considerando os princípios do INVEST:

- **I - Independent:** cada história representa uma necessidade específica.
- **N - Negotiable:** descreve o que o usuário precisa sem determinar uma solução técnica.
- **V - Valuable:** cada história apresenta um benefício para o usuário ou para o negócio.
- **E - Estimable:** possui escopo suficientemente claro para ser estimado.
- **S - Small:** as histórias possuem um objetivo específico e podem ser trabalhadas separadamente.
- **T - Testable:** possuem critérios de aceitação claros que permitem verificar se foram atendidas.
