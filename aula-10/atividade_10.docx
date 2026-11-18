# ESPECIFICAÇÃO DE REQUISITOS DE SOFTWARE
## Sistema de Delivery de Alimentos

### 1. Escopo

O sistema de delivery de alimentos tem como objetivo facilitar o processo de compra e entrega de refeições, conectando clientes, restaurantes e entregadores em uma única plataforma. Atualmente, o processo pode apresentar dificuldades na comunicação entre as partes, no acompanhamento dos pedidos e na atualização dos status da entrega. O sistema busca organizar essas etapas, permitindo que o cliente realize pedidos, acompanhe seu andamento e receba informações atualizadas até a entrega.

| Dentro do sistema | Fora do sistema |
|---|---|
| Cadastro e acesso dos clientes | Preparação física dos alimentos |
| Consulta de restaurantes e cardápios | Compra de ingredientes pelos restaurantes |
| Realização e confirmação de pedidos | Gerenciamento interno do estoque do restaurante |
| Processamento e confirmação de pagamentos | Administração financeira dos restaurantes |
| Atualização do status dos pedidos | Manutenção dos veículos dos entregadores |
| Acompanhamento da entrega | Trânsito e condições das vias públicas |
| Comunicação entre cliente, restaurante e entregador | Atendimento presencial no estabelecimento |

### 2. Processo

O processo começa quando o cliente acessa o sistema, escolhe um restaurante e seleciona os produtos desejados. Em seguida, adiciona os itens ao carrinho, informa o endereço de entrega e realiza o pagamento. Após a confirmação do pagamento, o pedido é encaminhado ao restaurante, que pode aceitá-lo ou recusá-lo. Caso seja aceito, o restaurante inicia a preparação e atualiza o status do pedido. Quando o alimento está pronto, um entregador realiza a retirada e inicia o transporte até o endereço informado. Durante esse período, o cliente pode acompanhar o andamento da entrega. Ao receber o pedido, o cliente confirma o recebimento e o processo é finalizado.

**Fluxo do processo:**

1. Cliente acessa o sistema.
2. Cliente escolhe um restaurante.
3. Cliente seleciona os produtos.
4. Sistema apresenta o resumo do pedido.
5. Cliente informa o endereço e realiza o pagamento.
6. Sistema confirma o pagamento.
7. Restaurante recebe o pedido.
8. Restaurante analisa e aceita ou recusa o pedido.
9. Se recusado, o sistema informa o cliente e inicia o procedimento de estorno, quando aplicável.
10. Se aceito, o restaurante prepara o pedido.
11. Entregador retira o pedido.
12. Entregador atualiza o status para "Em rota".
13. Cliente acompanha a entrega.
14. Entregador realiza a entrega.
15. Cliente confirma o recebimento.
16. Sistema finaliza o pedido.

### 3. Personas

**Mariana – Cliente**

Mariana trabalha durante o dia e possui pouco tempo para preparar refeições. Costuma utilizar aplicativos pelo celular para pedir comida, mas sente dificuldade quando não consegue acompanhar o andamento do pedido ou receber informações sobre possíveis atrasos. Seu principal objetivo é realizar pedidos de maneira rápida e acompanhar todas as etapas da entrega.

**Carlos – Responsável pelo restaurante**

Carlos administra um restaurante e recebe diversos pedidos diariamente. Precisa organizar os pedidos, verificar os produtos disponíveis e informar os clientes sobre o andamento da preparação. Sua principal dificuldade é manter a comunicação organizada durante os horários de maior movimento. Deseja utilizar um sistema que facilite o recebimento e o gerenciamento dos pedidos.

**Rafael – Entregador**

Rafael trabalha realizando entregas e utiliza o celular para consultar os endereços e acompanhar os pedidos disponíveis. Sua principal dificuldade é receber informações incompletas sobre as entregas e não conseguir comunicar rapidamente quando ocorre algum problema. Deseja visualizar os dados necessários e atualizar o status da entrega com facilidade.

### 4. Diagrama de casos de uso

O diagrama deverá representar o Sistema de Delivery de Alimentos, apresentando os atores que interagem com a plataforma e as principais funcionalidades disponíveis.

**Atores:**
- Cliente.
- Restaurante.
- Entregador.
- Serviço de pagamento (sistema externo).

**Casos de uso:**
- Realizar cadastro e login.
- Consultar restaurantes e cardápios.
- Realizar pedido.
- Efetuar pagamento.
- Acompanhar pedido.
- Aceitar ou recusar pedido.
- Atualizar status de preparação.
- Retirar pedido.
- Atualizar status da entrega.
- Confirmar recebimento.
- Informar problema na entrega.

### 5. Especificação do caso de uso

**Nome:** Realizar pedido.

**Ator principal:** Cliente.

**Gatilho:** O cliente deseja comprar uma refeição por meio do sistema.

**Pré-condição:** O cliente deve estar autenticado no sistema e possuir acesso a um restaurante disponível.

**Pós-condição:** O pedido fica registrado no sistema, com o pagamento processado ou aguardando confirmação, e é encaminhado ao restaurante após a confirmação do pagamento.

**Fluxo principal:**

1. O cliente acessa o sistema.
2. O sistema apresenta os restaurantes disponíveis.
3. O cliente seleciona um restaurante.
4. O sistema apresenta o cardápio.
5. O cliente escolhe os produtos desejados.
6. O cliente adiciona os produtos ao carrinho.
7. O sistema apresenta o resumo do pedido e o valor total.
8. O cliente informa o endereço de entrega.
9. O cliente seleciona a forma de pagamento.
10. O sistema encaminha a solicitação de pagamento ao serviço externo.
11. O serviço de pagamento confirma a transação.
12. O sistema registra o pedido e o encaminha ao restaurante.
13. O sistema informa ao cliente que o pedido foi enviado ao restaurante.

**Fluxo alternativo – Produto indisponível**

Quando: No passo 5, o cliente seleciona um produto que está indisponível.

1. O sistema informa que o produto não está disponível.
2. O cliente pode escolher outro produto ou removê-lo do pedido.
3. O sistema atualiza o carrinho.

Retorno: Volta ao passo 5.

**Exceções – Pagamento não aprovado**

Quando: No passo 11, o serviço de pagamento não confirma a transação.

1. O sistema informa ao cliente que o pagamento não foi aprovado.
2. O cliente pode escolher outra forma de pagamento ou tentar novamente.

Retorno: Volta ao passo 9. Caso o cliente desista, o pedido não é encaminhado ao restaurante.

### 6. Histórias e critérios de aceitação

**História 1 – Realizar pedido**

Como cliente, quero escolher produtos de um restaurante e realizar um pedido para receber minha refeição em casa.

| Dado que | Quando | Então |
|---|---|---|
| Estou autenticado no sistema | Seleciono um restaurante disponível | O sistema apresenta seu cardápio |
| Escolhi os produtos desejados | Confirmo o carrinho | O sistema apresenta o resumo e o valor total |
| Informei o endereço e a forma de pagamento | O pagamento é aprovado | O sistema registra e encaminha o pedido ao restaurante |

**História 2 – Gerenciar pedido**

Como responsável pelo restaurante, quero receber e analisar os pedidos para organizar a preparação das refeições.

| Dado que | Quando | Então |
|---|---|---|
| Existe um novo pedido | Acesso a lista de pedidos | O sistema apresenta os dados do pedido |
| Recebi um pedido | Confirmo sua aceitação | O sistema atualiza o status para aceito |
| Recebi um pedido | Recuso o pedido informando o motivo | O sistema comunica a recusa ao cliente |

**História 3 – Acompanhar pedido**

Como cliente, quero acompanhar o status do meu pedido para saber em qual etapa ele está.

| Dado que | Quando | Então |
|---|---|---|
| Realizei um pedido | Acesso à área de acompanhamento | O sistema apresenta o status atual |
| O restaurante iniciou a preparação | Consulto o pedido | O sistema apresenta o status em preparação |
| O entregador iniciou a entrega | Consulto o pedido | O sistema apresenta o status em rota |

**História 4 – Realizar entrega**

Como entregador, quero visualizar os pedidos destinados à entrega e atualizar seus status para manter o cliente informado.

| Dado que | Quando | Então |
|---|---|---|
| Existe um pedido pronto | Acesso aos pedidos disponíveis para retirada | O sistema apresenta os dados da entrega |
| Retirei o pedido no restaurante | Atualizo o status da entrega | O sistema informa que o pedido está em rota |
| Entreguei o pedido ao cliente | Confirmo a entrega | O sistema registra a conclusão do pedido |

**História 5 – Informar problema na entrega**

Como entregador, quero informar problemas ocorridos durante a entrega para que o cliente e o sistema sejam atualizados.

| Dado que | Quando | Então |
|---|---|---|
| Estou realizando uma entrega | Identifico um problema | O sistema disponibiliza a opção de informar ocorrência |
| Ocorreu um problema na entrega | Registro a descrição da ocorrência | O sistema armazena e comunica a informação |
| A ocorrência foi registrada | O cliente consulta o pedido | O sistema apresenta a atualização disponível |

### 7. Regras de negócio

| Regra | Descrição | Origem |
|---|---|---|
| RN01 – Cadastro | O cliente deve possuir cadastro e autenticação para realizar pedidos. | Política do sistema |
| RN02 – Disponibilidade | Somente produtos disponíveis podem ser adicionados ao pedido. | Política do restaurante |
| RN03 – Pagamento | O pedido somente será encaminhado ao restaurante após a confirmação do pagamento, quando a modalidade exigir pagamento antecipado. | Política de pagamento |
| RN04 – Aceitação | O restaurante deve aceitar ou recusar o pedido antes de iniciar sua preparação. | Processo operacional |
| RN05 – Atualização | O status do pedido deve ser atualizado conforme as etapas de preparação e entrega. | Política do sistema |
| RN06 – Entrega | O entregador deve confirmar a retirada e a conclusão da entrega no sistema. | Processo operacional |
| RN07 – Ocorrências | Problemas identificados durante a entrega devem ser registrados para manter o cliente informado. | Política do sistema |
| RN08 – Privacidade | Os dados pessoais dos clientes devem ser tratados de acordo com a legislação de proteção de dados. | LGPD – Lei nº 13.709/2018 |
