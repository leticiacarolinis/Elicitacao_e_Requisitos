# Aula 9 – Personas e casos de uso

## Sistema escolhido: Sistema de Delivery de Alimentos

O sistema permite que clientes consultem o cardápio de restaurantes, realizem pedidos e acompanhem o andamento da entrega. Os restaurantes podem gerenciar a disponibilidade dos itens e atualizar o status dos pedidos. O pagamento é processado por um serviço externo.

## Atores

- **Cliente (ator principal):** consulta o cardápio, realiza pedidos e acompanha o andamento dos pedidos.
- **Restaurante (ator principal):** gerencia a disponibilidade dos itens do cardápio e atualiza o status dos pedidos.
- **Gateway de pagamento (ator secundário):** serviço externo responsável por autorizar ou recusar as transações de pagamento.

## Casos de uso representados

1. **Consultar cardápio:** permite ao cliente visualizar os produtos e verificar quais estão disponíveis.
2. **Realizar pedido:** permite ao cliente selecionar os itens, informar os dados necessários e concluir o pedido após a aprovação do pagamento.
3. **Acompanhar pedido:** permite ao cliente consultar o status do pedido, como recebido, em preparação e saiu para entrega.
4. **Gerenciar disponibilidade dos itens:** permite ao restaurante indicar quais produtos estão disponíveis ou indisponíveis.
5. **Atualizar status do pedido:** permite ao restaurante informar a situação do pedido.
6. **Processar pagamento:** solicita ao gateway externo a autorização do pagamento. Esse caso de uso é incluído em “Realizar pedido”.

## Especificação do caso de uso: Realizar pedido

**Ator:** Cliente.

**Descrição:** permite que o cliente selecione produtos disponíveis no cardápio, informe o endereço de entrega, escolha a forma de pagamento e envie o pedido ao restaurante.

**Gatilho:** o cliente decide comprar um ou mais produtos e seleciona a opção para realizar o pedido.

**Pré-condições:**
- O cliente deve estar autenticado no sistema.
- Deve existir ao menos um restaurante com cardápio disponível.
- Os itens escolhidos devem estar disponíveis no momento da confirmação.

**Pós-condições:**
- O pedido é registrado no sistema com um número de identificação.
- O pagamento é autorizado.
- O restaurante recebe o pedido para iniciar o atendimento.

### Fluxo principal

1. O cliente acessa o cardápio de um restaurante.
2. O sistema apresenta os produtos disponíveis e seus preços.
3. O cliente seleciona os produtos e suas quantidades.
4. O sistema adiciona os produtos ao carrinho e apresenta o resumo do pedido.
5. O cliente confirma o pedido e informa ou seleciona o endereço de entrega.
6. O sistema apresenta as formas de pagamento disponíveis.
7. O cliente seleciona uma forma de pagamento e informa os dados solicitados.
8. O sistema envia a solicitação de pagamento ao gateway de pagamento.
9. O gateway autoriza a transação e retorna a confirmação ao sistema.
10. O sistema registra o pedido e o encaminha ao restaurante.
11. O sistema apresenta ao cliente a confirmação e o número do pedido.

### Fluxo alternativo – Alterar quantidade de um produto

**Quando ocorre:** no momento em que o cliente está conferindo os produtos no carrinho, antes de confirmar o pedido.

1. O cliente identifica que deseja alterar a quantidade de um produto.
2. O cliente aumenta ou diminui a quantidade do produto no carrinho.
3. O sistema atualiza a quantidade e recalcula o valor total.
4. O sistema apresenta o carrinho atualizado.

**Retorno:** o fluxo retorna ao passo 5 do fluxo principal, para que o cliente confirme o pedido e informe o endereço de entrega.

### Exceção – Pagamento não autorizado

**Quando ocorre:** após o envio da solicitação de pagamento, quando o gateway recusa a transação ou não consegue autorizá-la.

1. O gateway informa que o pagamento não foi autorizado.
2. O sistema comunica ao cliente que o pagamento não foi concluído.
3. O sistema mantém o pedido sem confirmação e apresenta a opção de tentar novamente com outra forma de pagamento.
4. O cliente seleciona outra forma de pagamento ou decide cancelar a operação.

**Retorno:** se o cliente escolher tentar novamente, o fluxo retorna ao passo 6 do fluxo principal. Se cancelar, o caso de uso é encerrado sem registrar o pedido como confirmado.
