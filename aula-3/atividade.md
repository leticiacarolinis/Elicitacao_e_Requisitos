# Atividade - Requisitos Não Funcionais

## Disciplina

Elicitação de Requisitos

## Aula 3

---

## História 1 - Avaliação do pedido

**História de usuário:**

Como cliente, quero avaliar o pedido depois da entrega, para ajudar outros clientes a escolherem melhor.

### RNF 1 - Desempenho

O sistema deve carregar a opção de avaliação em até 2 segundos após o cliente abrir o aplicativo com o pedido já entregue.

**Característica da ISO/IEC 25010:** Eficiência de desempenho.

### RNF 2 - Usabilidade

A opção de avaliação deve ser apresentada de forma clara e fácil de localizar, permitindo que o cliente compreenda como realizar a avaliação sem precisar de instruções externas.

**Característica da ISO/IEC 25010:** Usabilidade.

### RNF 3 - Confiabilidade

O sistema deve garantir que a avaliação enviada pelo cliente seja registrada corretamente e permaneça disponível no perfil do restaurante após a confirmação do envio.

**Característica da ISO/IEC 25010:** Confiabilidade.

---

## História 2 - Salvar cartão de pagamento

**História de usuário:**

Como cliente, quero salvar um cartão de pagamento, para não digitar os dados a cada compra.

### RNF 4 - Segurança

Os dados do cartão salvo devem ser protegidos contra acesso não autorizado durante o armazenamento e utilização no aplicativo.

**Característica da ISO/IEC 25010:** Segurança.

### RNF 5 - Usabilidade

O cadastro de um cartão deve apresentar campos e instruções claras, permitindo que o cliente realize o cadastro de forma simples.

**Característica da ISO/IEC 25010:** Usabilidade.

### RNF 6 - Confiabilidade

O sistema deve manter o cartão cadastrado disponível para seleção no checkout enquanto ele estiver válido e não for removido pelo cliente.

**Característica da ISO/IEC 25010:** Confiabilidade.

---

## História 3 - Resumo diário de vendas

**História de usuário:**

Como dono de restaurante, quero ver um resumo diário de vendas, para acompanhar o desempenho do dia.

### RNF 7 - Desempenho

O resumo de vendas deve ser carregado em até 3 segundos após o restaurante abrir o painel de vendas.

**Característica da ISO/IEC 25010:** Eficiência de desempenho.

### RNF 8 - Adequação funcional

O resumo de vendas deve apresentar corretamente o total de pedidos e o faturamento correspondente ao período selecionado.

**Característica da ISO/IEC 25010:** Adequação funcional.

### RNF 9 - Usabilidade

O painel de vendas deve apresentar as informações de pedidos e faturamento de forma organizada e compreensível, facilitando a consulta pelo dono do restaurante.

**Característica da ISO/IEC 25010:** Usabilidade.

---

## Resumo dos RNF

| História | RNF | Característica da ISO/IEC 25010 |
|---|---|---|
| História 1 - Avaliação do pedido | Carregamento da avaliação em até 2 segundos | Eficiência de desempenho |
| História 1 - Avaliação do pedido | Opção de avaliação clara e fácil de localizar | Usabilidade |
| História 1 - Avaliação do pedido | Registro correto da avaliação | Confiabilidade |
| História 2 - Salvar cartão | Proteção dos dados do cartão | Segurança |
| História 2 - Salvar cartão | Cadastro simples e claro | Usabilidade |
| História 2 - Salvar cartão | Disponibilidade do cartão salvo | Confiabilidade |
| História 3 - Resumo de vendas | Carregamento do resumo em até 3 segundos | Eficiência de desempenho |
| História 3 - Resumo de vendas | Apresentação correta dos dados | Adequação funcional |
| História 3 - Resumo de vendas | Informações organizadas e compreensíveis | Usabilidade |
